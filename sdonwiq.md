代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://ap.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xl.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://eq.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qc.bjjhwx.cn

[C02] 默认参数
来源：http://qi.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://mi.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dq.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://xk.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ik.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://et.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fl.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://uq.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://uk.asd995.cn

[C03] 可变参数
来源：http://tf.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://vk.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nz.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ne.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fn.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://as.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ne.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bn.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vn.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://tp.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://np.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ts.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://so.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tq.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://mw.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://de.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://wb.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://ic.yuexingan06.cn

[C05] 返回多个值
来源：http://oe.jianghongdianzi.cn

Py:   return a, b
来源：http://lf.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://eh.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://of.muxihuayi.cn

TS:   return { a, b };
来源：http://cc.yuntaijiaju.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pi.jctech888.com.cn

Go:   return a, b
来源：http://or.chemitech.net.cn

Ruby: return a, b
来源：http://uu.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://oh.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://ch.huanxung.cn

Py:   square = lambda x: x * x
来源：http://dw.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pu.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://et.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://lv.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://az.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uh.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://zk.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zk.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://en.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bm.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cf.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kk.bjjhwx.cn

TS:   arr.map(String)
来源：http://ti.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xo.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ad.521024.cn

Ruby: arr.map(&:upcase)
来源：http://vb.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wr.huixinmuqiang.cn

[C08] 闭包
来源：http://eq.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yg.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pt.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://me.521024.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ex.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aj.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://or.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qy.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dn.huixiangedu.cn

[C09] 递归
来源：http://vv.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vt.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mo.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://or.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bc.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pw.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vj.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yo.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sy.panjiajie.cn

[C10] 变量作用域
来源：http://bh.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vz.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dk.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dh.panjiajie.cn

TS:   同 JS
来源：http://oo.lnxyls.cn

Java: 方法内为块级作用域
来源：http://uh.jctech888.com.cn

Go:   花括号块级作用域
来源：http://vh.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gv.muxihuayi.cn

C#:   块级作用域
来源：http://tl.shxzskj.cn

[C11] 模块导入与导出
来源：http://ic.bjjhwx.cn

Py:   from module import func
来源：http://nd.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bk.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rf.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ce.huanxung.cn

Java: import java.util.List;
来源：http://ki.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nm.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://te.521024.cn

C#:   using System.Text;
来源：http://sc.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://vs.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://hi.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://id.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://um.gzmigu.cn

TS:   (() => { console.log("run"); })();
来源：http://ff.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ua.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://dh.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://mz.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cx.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://br.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nu.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sg.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vx.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ix.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rd.newstarts.cn

Go:   func add(a, b int) int
来源：http://fb.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ar.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bx.huixiangedu.cn

[C14] 泛型函数
来源：http://lv.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fy.newstarts.cn

PHP:  // 无泛型
来源：http://xn.nicolike.cn

JS:   // 无泛型
来源：http://yr.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wv.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://em.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://my.colortex.cn

Ruby: # 无泛型
来源：http://dr.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://in.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://lj.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bl.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://nc.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hf.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ig.muxihuayi.cn

Java: // 无解构
来源：http://kg.shtwfgs.cn

Go:   // 无解构
来源：http://hp.muxihuayi.cn

Ruby: a, b = pair
来源：http://hw.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://fd.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://ie.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sp.huanxung.cn

PHP:  // 无重载
来源：http://sz.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fy.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://rj.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ip.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://re.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://ri.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://do.hahajie.cn

================================================================================
来源：http://cb.asd995.cn

D. 数组 / 列表 / 集合
来源：http://eu.521024.cn

================================================================================
来源：http://hz.newstarts.cn

[D01] 创建数组 / 列表
来源：http://nw.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bb.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ac.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fx.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bf.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://na.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://iq.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://cl.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zr.nicolike.cn

[D02] 追加元素到末尾
来源：http://kc.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mh.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qu.asd995.cn

JS:   arr.push(4);
来源：http://ih.jctech888.com.cn

TS:   arr.push(4);
来源：http://ui.panjiajie.cn

Java: list.add(4);
来源：http://zh.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://ul.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://uf.asd995.cn

C#:   list.Add(4);
来源：http://ir.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://ui.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://gv.panjiajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gi.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nb.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://hr.szxytkj.cn

Java: list.add(0, 0);
来源：http://in.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ee.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://io.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://rm.muxihuayi.cn

[D04] 删除元素
来源：http://un.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kh.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ck.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bv.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://il.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ct.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lv.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iu.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://az.haigaiapp.cn

[D05] 访问与修改元素
来源：http://dl.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tk.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aa.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qh.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://kw.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://bm.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://cu.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ak.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bu.bjjhwx.cn

[D06] 数组长度
来源：http://bu.yuexingan06.cn

Py:   len(arr)
来源：http://ye.asd995.cn

PHP:  count($arr);
来源：http://pr.huanxung.cn

JS:   arr.length
来源：http://kp.colortex.cn

TS:   arr.length
来源：http://fi.hahajie.cn

Java: list.size();
来源：http://ur.9csxet.cn

Go:   len(arr)
来源：http://ai.asd995.cn

Ruby: arr.length; arr.size
来源：http://rd.muxihuayi.cn

C#:   list.Count;
来源：http://pk.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://yc.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ou.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gk.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://bw.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://bw.gzmigu.cn

Java: list.subList(1, 4);
来源：http://gf.szsharing.cn

Go:   arr[1:4]
来源：http://yr.lnxyls.cn

Ruby: arr[1, 3]
来源：http://dm.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://jw.colortex.cn

[D08] 合并两个数组
来源：http://ow.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://jh.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://qj.colortex.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fw.shxzukj.cn

TS:   [...a, ...b];
来源：http://ha.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vi.nszjky.cn

Go:   append(a, b...)
来源：http://qm.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://fj.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://co.521024.cn

[D09] 排序（升序）
来源：http://uq.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://mv.9csxet.cn

PHP:  sort($arr);
来源：http://ok.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wl.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gs.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bo.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bj.9csxet.cn

Ruby: arr.sort
来源：http://mr.hnjuh.cn

C#:   list.Sort();
来源：http://tw.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gz.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mv.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oe.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oh.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sx.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pt.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ld.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uy.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ul.shxzukj.cn

[D11] 反转数组
来源：http://hm.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cn.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://dh.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xr.nicolike.cn

TS:   [...arr].reverse();
来源：http://ca.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://zy.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://mn.haigaiapp.cn

Ruby: arr.reverse
来源：http://eo.wgjwhj.cn

C#:   list.Reverse();
来源：http://wk.huanxung.cn

[D12] 查找元素下标
来源：http://bi.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://ov.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ev.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sj.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fb.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lb.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://vi.nszjky.cn

Ruby: arr.index(x)
来源：http://wl.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://km.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://qe.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cw.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://do.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://xr.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://ew.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rv.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tj.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wk.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ta.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://em.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ak.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cn.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://jr.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://sl.wgjwhj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kv.bookmarksfly.cn

Go:   // 手写循环
来源：http://ea.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jc.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vs.huixinmuqiang.cn

[D15] 去重
来源：http://rt.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://so.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://lm.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://gz.newstarts.cn

TS:   [...new Set(arr)]
来源：http://cg.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://im.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mb.hnjuh.cn

Ruby: arr.uniq
来源：http://sz.colortex.cn

C#:   list.Distinct().ToList()
来源：http://aa.lnxyls.cn

[D16] 求和与平均值
来源：http://ff.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bt.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dm.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ho.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ec.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iy.gzmigu.cn

Go:   // 手写循环累加
来源：http://ql.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yc.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://ta.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://ij.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://gy.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://pe.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tu.nszjky.cn

TS:   Math.max(...arr);
来源：http://iq.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vo.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ll.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://kg.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://dk.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://xk.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ls.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://bv.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qf.wgjwhj.cn

TS:   nested.flat();
来源：http://xp.jianghongdianzi.cn


<!-- 参考信息 -->