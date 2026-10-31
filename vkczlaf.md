代发 wailian999

================================================================================
来源：http://hl.muxihuayi.cn

C. 函数与作用域
来源：http://ku.nicolike.cn

================================================================================
来源：http://lj.chemitech.net.cn

[C01] 定义函数
来源：http://ci.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://kl.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xd.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://nd.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ov.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xh.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vs.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://xv.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yw.colortex.cn

[C02] 默认参数
来源：http://lk.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://fo.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://je.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://gy.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bh.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jr.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ut.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://ev.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://tx.szsharing.cn

[C03] 可变参数
来源：http://ub.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://ct.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jw.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xi.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lb.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sk.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nz.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pk.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oe.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://tj.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ma.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jv.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ui.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oe.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://qg.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://xp.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://mp.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://ct.szsharing.cn

[C05] 返回多个值
来源：http://to.hnjuh.cn

Py:   return a, b
来源：http://oj.huanxung.cn

PHP:  return [$a, $b];
来源：http://sz.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://af.9csxet.cn

TS:   return { a, b };
来源：http://yp.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sr.huixiangedu.cn

Go:   return a, b
来源：http://vj.bjjhwx.cn

Ruby: return a, b
来源：http://fa.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://dg.521024.cn

[C06] 匿名函数 / lambda
来源：http://vc.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://bq.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sp.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://gd.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://bw.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hk.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tx.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://yh.shxzukj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qd.nszjky.cn

[C07] 把函数作为参数传入
来源：http://fc.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://et.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yw.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oz.hnjuh.cn

TS:   arr.map(String)
来源：http://fp.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://px.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ad.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://ua.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://le.haigaiapp.cn

[C08] 闭包
来源：http://mo.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yu.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zn.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xw.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gu.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lj.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eg.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gn.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mr.haigaiapp.cn

[C09] 递归
来源：http://kp.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rz.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iy.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://su.gzmigu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hw.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gg.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ho.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ih.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ti.huixinmuqiang.cn

[C10] 变量作用域
来源：http://ee.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xj.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ca.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ux.jctech888.com.cn

TS:   同 JS
来源：http://ai.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://xo.wgjwhj.cn

Go:   花括号块级作用域
来源：http://ri.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ly.haigaiapp.cn

C#:   块级作用域
来源：http://os.panjiajie.cn

[C11] 模块导入与导出
来源：http://ep.yuntaijiaju.cn

Py:   from module import func
来源：http://sd.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tn.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wm.huanxung.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dz.huixiangedu.cn

Java: import java.util.List;
来源：http://bm.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lx.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://mh.panjiajie.cn

C#:   using System.Text;
来源：http://nw.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://ff.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://je.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://yj.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://jj.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://wa.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ui.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://xi.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://qu.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ii.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://cj.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aq.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vd.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pf.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ua.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fq.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://fr.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uf.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yh.jianghongdianzi.cn

[C14] 泛型函数
来源：http://kl.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ar.hahajie.cn

PHP:  // 无泛型
来源：http://fc.bjjhwx.cn

JS:   // 无泛型
来源：http://ja.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pc.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ko.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wl.hnjuh.cn

Ruby: # 无泛型
来源：http://ev.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sg.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://km.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://me.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://yz.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ir.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pq.yuexingan06.cn

Java: // 无解构
来源：http://vj.nicolike.cn

Go:   // 无解构
来源：http://xs.nicolike.cn

Ruby: a, b = pair
来源：http://qf.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://xx.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://lx.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ft.muxihuayi.cn

PHP:  // 无重载
来源：http://xq.nszjky.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yu.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://yj.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bn.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://td.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://uv.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ca.asd995.cn

================================================================================
来源：http://jz.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://ak.hnjuh.cn

================================================================================
来源：http://gc.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://je.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://eu.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zo.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ht.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bq.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ro.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://ap.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://fr.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://as.newstarts.cn

[D02] 追加元素到末尾
来源：http://ov.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ia.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ow.9csxet.cn

JS:   arr.push(4);
来源：http://ij.szsharing.cn

TS:   arr.push(4);
来源：http://wq.huixinmuqiang.cn

Java: list.add(4);
来源：http://pc.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://lt.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://uw.muxihuayi.cn

C#:   list.Add(4);
来源：http://bo.9csxet.cn

[D03] 在指定位置插入元素
来源：http://kr.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://gw.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tm.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vj.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://iy.newstarts.cn

Java: list.add(0, 0);
来源：http://zz.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qj.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mo.521024.cn

C#:   list.Insert(0, 0);
来源：http://id.szsharing.cn

[D04] 删除元素
来源：http://bi.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ah.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wm.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rt.asd995.cn

TS:   arr.splice(0, 1);
来源：http://yr.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ae.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dm.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fs.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ji.huixiangedu.cn

[D05] 访问与修改元素
来源：http://qw.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gg.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ru.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yy.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://fp.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://vl.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://jl.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dl.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://im.huixiangedu.cn

[D06] 数组长度
来源：http://bm.panjiajie.cn

Py:   len(arr)
来源：http://sc.lnxyls.cn

PHP:  count($arr);
来源：http://fa.asd995.cn

JS:   arr.length
来源：http://de.yuntaijiaju.cn

TS:   arr.length
来源：http://kv.9csxet.cn

Java: list.size();
来源：http://kd.gzmigu.cn

Go:   len(arr)
来源：http://cb.szsharing.cn

Ruby: arr.length; arr.size
来源：http://sd.bjjhwx.cn

C#:   list.Count;
来源：http://sq.asd995.cn

[D07] 切片 / 取子数组
来源：http://jd.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ea.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wz.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://cf.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://fn.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://kr.szxytkj.cn

Go:   arr[1:4]
来源：http://wb.gzmigu.cn

Ruby: arr[1, 3]
来源：http://ey.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://xu.szxytkj.cn

[D08] 合并两个数组
来源：http://vs.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://sw.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://qd.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lo.shxzskj.cn

TS:   [...a, ...b];
来源：http://ui.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ig.wgjwhj.cn

Go:   append(a, b...)
来源：http://md.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://hh.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://mh.shxzskj.cn

[D09] 排序（升序）
来源：http://ix.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://qj.jctech888.com.cn

PHP:  sort($arr);
来源：http://pn.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ji.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lv.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://th.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sy.shtwfgs.cn

Ruby: arr.sort
来源：http://yi.shxzskj.cn

C#:   list.Sort();
来源：http://gk.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uk.colortex.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ac.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xi.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sm.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zs.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zj.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pa.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uh.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hy.colortex.cn

[D11] 反转数组
来源：http://rx.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gm.nicolike.cn

PHP:  array_reverse($arr);
来源：http://zv.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://km.521024.cn

TS:   [...arr].reverse();
来源：http://dd.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://kr.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://dk.chemitech.net.cn

Ruby: arr.reverse
来源：http://yi.nicolike.cn

C#:   list.Reverse();
来源：http://ij.nszjky.cn

[D12] 查找元素下标
来源：http://ar.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://zg.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kf.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sy.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pq.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sm.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://fj.yuexingan06.cn

Ruby: arr.index(x)
来源：http://sx.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://lt.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://dg.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rj.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eg.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://kc.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://dd.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ag.panjiajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://au.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ep.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hb.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://in.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wn.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gj.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://nm.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://wp.wgjwhj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wt.asd995.cn

Go:   // 手写循环
来源：http://ge.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zd.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://te.szxytkj.cn

[D15] 去重
来源：http://es.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://aa.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://ug.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://ok.9csxet.cn

TS:   [...new Set(arr)]
来源：http://xy.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kr.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gm.bjjhwx.cn

Ruby: arr.uniq
来源：http://jy.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://ny.nszjky.cn

[D16] 求和与平均值
来源：http://gf.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uh.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lb.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iu.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fa.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eh.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://tf.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hy.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://cd.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://fd.asd995.cn

Py:   max(arr);  min(arr)
来源：http://nn.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://by.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tx.nszjky.cn

TS:   Math.max(...arr);
来源：http://bi.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xa.nszjky.cn


<!-- 参考信息 -->