代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://il.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://li.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wh.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://yd.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://yc.shxzskj.cn

[C03] 可变参数
来源：http://rc.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://fy.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://de.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ih.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://le.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iw.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bo.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://or.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yv.shxzukj.cn

[C04] 命名参数 / 关键字参数
来源：http://pv.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ju.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tc.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://om.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ji.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://lj.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://fj.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://qe.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://jz.colortex.cn

[C05] 返回多个值
来源：http://dl.jctech888.com.cn

Py:   return a, b
来源：http://er.521024.cn

PHP:  return [$a, $b];
来源：http://wt.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pu.huanxung.cn

TS:   return { a, b };
来源：http://ff.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ej.asd995.cn

Go:   return a, b
来源：http://mq.hahajie.cn

Ruby: return a, b
来源：http://fl.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://th.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://bj.asd995.cn

Py:   square = lambda x: x * x
来源：http://ty.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hl.panjiajie.cn

JS:   const square = x => x * x;
来源：http://te.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://bm.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qa.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sv.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://zm.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ry.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://fa.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hx.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tz.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sl.jctech888.com.cn

TS:   arr.map(String)
来源：http://nr.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cj.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lt.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://cb.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kn.gzmigu.cn

[C08] 闭包
来源：http://dr.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vs.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lz.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://op.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jm.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nm.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://us.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tq.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ma.szsharing.cn

[C09] 递归
来源：http://ab.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://if.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ry.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cn.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qq.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mr.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://is.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ed.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bu.jctech888.com.cn

[C10] 变量作用域
来源：http://er.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://le.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ew.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hp.szxytkj.cn

TS:   同 JS
来源：http://sf.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://hw.szxytkj.cn

Go:   花括号块级作用域
来源：http://vj.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nv.muxihuayi.cn

C#:   块级作用域
来源：http://aw.hnjuh.cn

[C11] 模块导入与导出
来源：http://ld.yuntaijiaju.cn

Py:   from module import func
来源：http://tw.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tp.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://me.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lr.521024.cn

Java: import java.util.List;
来源：http://nk.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nb.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://eq.nszjky.cn

C#:   using System.Text;
来源：http://wz.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://ad.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://wb.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://sy.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://rm.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://id.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zg.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://cd.bookmarksfly.cn

Ruby: -> { puts "run" }.call
来源：http://kg.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uo.521024.cn

[C13] 类型声明 / 类型注解
来源：http://qn.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zi.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://is.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gl.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vg.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sy.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://mu.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rp.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bs.haigaiapp.cn

[C14] 泛型函数
来源：http://ec.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fi.521024.cn

PHP:  // 无泛型
来源：http://kf.szsharing.cn

JS:   // 无泛型
来源：http://sy.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ne.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gv.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zj.yuexingan06.cn

Ruby: # 无泛型
来源：http://fy.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://um.nicolike.cn

[C15] 解构 / 展开参数
来源：http://xu.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hf.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://zr.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gc.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vb.nszjky.cn

Java: // 无解构
来源：http://vr.wgjwhj.cn

Go:   // 无解构
来源：http://dy.nszjky.cn

Ruby: a, b = pair
来源：http://sg.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://dw.shxzukj.cn

[C16] 函数 / 方法重载
来源：http://ky.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://za.shtwfgs.cn

PHP:  // 无重载
来源：http://gp.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sw.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://vl.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ky.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://wf.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://gz.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vq.shtwfgs.cn

================================================================================
来源：http://am.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://ak.panjiajie.cn

================================================================================
来源：http://pm.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://gw.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tn.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hv.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kz.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zh.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://om.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://yw.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://cp.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fw.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://rw.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wm.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zh.szxytkj.cn

JS:   arr.push(4);
来源：http://np.lnxyls.cn

TS:   arr.push(4);
来源：http://fx.haigaiapp.cn

Java: list.add(4);
来源：http://hk.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://rs.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://cu.szxytkj.cn

C#:   list.Add(4);
来源：http://pg.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://if.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://ck.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qd.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kb.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://cw.wgjwhj.cn

Java: list.add(0, 0);
来源：http://ke.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://at.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rm.asd995.cn

C#:   list.Insert(0, 0);
来源：http://ij.shxzskj.cn

[D04] 删除元素
来源：http://ws.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gd.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rr.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oz.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://cq.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bb.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rs.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yz.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.newstarts.cn

[D05] 访问与修改元素
来源：http://lw.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tc.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jv.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ja.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://nf.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://tc.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://dw.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iv.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://df.jianghongdianzi.cn

[D06] 数组长度
来源：http://fd.chemitech.net.cn

Py:   len(arr)
来源：http://nk.panjiajie.cn

PHP:  count($arr);
来源：http://fq.lnxyls.cn

JS:   arr.length
来源：http://bi.nszjky.cn

TS:   arr.length
来源：http://fc.jctech888.com.cn

Java: list.size();
来源：http://dw.bookmarksfly.cn

Go:   len(arr)
来源：http://xm.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://yu.jctech888.com.cn

C#:   list.Count;
来源：http://di.nicolike.cn

[D07] 切片 / 取子数组
来源：http://rt.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jv.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vf.colortex.cn

JS:   arr.slice(1, 4);
来源：http://uq.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://gu.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://ix.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://hs.szxytkj.cn

Ruby: arr[1, 3]
来源：http://vx.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://ry.szsharing.cn

[D08] 合并两个数组
来源：http://co.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://pt.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://ur.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dc.521024.cn

TS:   [...a, ...b];
来源：http://tl.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ix.521024.cn

Go:   append(a, b...)
来源：http://gp.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://cp.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://pm.hnjuh.cn

[D09] 排序（升序）
来源：http://vq.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://iz.szsharing.cn

PHP:  sort($arr);
来源：http://ym.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://by.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://is.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ps.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ok.haigaiapp.cn

Ruby: arr.sort
来源：http://gh.newstarts.cn

C#:   list.Sort();
来源：http://vm.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bw.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pb.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wz.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wm.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ac.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://np.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ld.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fm.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hm.bjjhwx.cn

[D11] 反转数组
来源：http://sm.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://iw.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://dh.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://or.shxzskj.cn

TS:   [...arr].reverse();
来源：http://zs.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://ck.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://ot.shxzukj.cn

Ruby: arr.reverse
来源：http://tk.newstarts.cn

C#:   list.Reverse();
来源：http://vb.huixiangedu.cn

[D12] 查找元素下标
来源：http://ll.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://ys.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pp.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ay.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pp.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gc.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://xo.hahajie.cn

Ruby: arr.index(x)
来源：http://wd.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://ff.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://zk.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ot.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hw.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://ky.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://vx.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dd.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gb.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mx.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fd.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://ew.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kc.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qp.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://li.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://ls.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yz.nicolike.cn

Go:   // 手写循环
来源：http://lw.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bq.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vl.szsharing.cn

[D15] 去重
来源：http://dj.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kw.hnjuh.cn

PHP:  array_unique($arr);
来源：http://ox.colortex.cn

JS:   [...new Set(arr)]
来源：http://jk.newstarts.cn

TS:   [...new Set(arr)]
来源：http://uh.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yw.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wo.haigaiapp.cn

Ruby: arr.uniq
来源：http://tz.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://pc.asd995.cn

[D16] 求和与平均值
来源：http://kl.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tx.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yt.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rj.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yv.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bx.szxytkj.cn

Go:   // 手写循环累加
来源：http://ol.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qk.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://tq.chemitech.net.cn

[D17] 最大值与最小值
来源：http://tw.asd995.cn

Py:   max(arr);  min(arr)
来源：http://gq.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://vc.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lv.hnjuh.cn

TS:   Math.max(...arr);
来源：http://bu.newstarts.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ok.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dx.szxytkj.cn

Ruby: arr.max;  arr.min
来源：http://pm.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://vb.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://nr.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qo.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://hi.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xe.shxzskj.cn

TS:   nested.flat();
来源：http://sm.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ef.wgjwhj.cn

Go:   // 手写双层循环
来源：http://he.shtwfgs.cn

Ruby: nested.flatten
来源：http://kj.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rw.huanxung.cn

[D19] 按字段分组
来源：http://lp.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ix.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://af.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ij.lnxyls.cn


<!-- 参考信息 -->