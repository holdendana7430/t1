代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://ou.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hg.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nm.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://ih.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://ri.lnxyls.cn

[C03] 可变参数
来源：http://vc.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://zl.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nm.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jv.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pa.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zq.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mp.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ga.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://az.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://kl.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://is.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fo.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uh.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ht.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://bv.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://zn.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://gm.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://ya.521024.cn

[C05] 返回多个值
来源：http://yo.gzmigu.cn

Py:   return a, b
来源：http://kq.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://jn.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gf.newstarts.cn

TS:   return { a, b };
来源：http://bc.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wn.huanxung.cn

Go:   return a, b
来源：http://vg.yuntaijiaju.cn

Ruby: return a, b
来源：http://ge.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://dt.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://zj.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://rx.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yg.panjiajie.cn

JS:   const square = x => x * x;
来源：http://ik.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://qe.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pk.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oy.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://id.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ai.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://bo.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ln.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ck.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hc.shxzukj.cn

TS:   arr.map(String)
来源：http://yg.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qa.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cs.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://pw.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tu.colortex.cn

[C08] 闭包
来源：http://kr.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://it.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wf.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ya.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uk.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vh.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qp.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qu.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hc.chemitech.net.cn

[C09] 递归
来源：http://pm.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rf.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lo.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uw.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ip.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lr.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pi.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pc.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ky.bjjhwx.cn

[C10] 变量作用域
来源：http://fx.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ni.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://to.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hq.jctech888.com.cn

TS:   同 JS
来源：http://tf.nicolike.cn

Java: 方法内为块级作用域
来源：http://oe.szxytkj.cn

Go:   花括号块级作用域
来源：http://ar.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kk.521024.cn

C#:   块级作用域
来源：http://cw.huixiangedu.cn

[C11] 模块导入与导出
来源：http://es.yuexingan06.cn

Py:   from module import func
来源：http://dq.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qo.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bk.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://im.shtwfgs.cn

Java: import java.util.List;
来源：http://kr.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fi.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://ms.lnxyls.cn

C#:   using System.Text;
来源：http://rj.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://ed.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://mj.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://nh.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://ee.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://qy.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aa.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://oo.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://sr.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dx.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://hl.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ui.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pq.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cp.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yv.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ie.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://ej.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ns.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ww.shxzukj.cn

[C14] 泛型函数
来源：http://ao.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fu.szxytkj.cn

PHP:  // 无泛型
来源：http://bl.jianghongdianzi.cn

JS:   // 无泛型
来源：http://gx.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fm.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ec.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jh.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://bf.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wl.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://vr.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ty.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://gk.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gw.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ph.hnjuh.cn

Java: // 无解构
来源：http://gn.szsharing.cn

Go:   // 无解构
来源：http://dl.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://la.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://iv.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://wn.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rw.gzmigu.cn

PHP:  // 无重载
来源：http://qy.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zz.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://uz.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ih.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://rp.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://kx.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://re.nszjky.cn

================================================================================
来源：http://it.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://jw.huixiangedu.cn

================================================================================
来源：http://mb.chemitech.net.cn

[D01] 创建数组 / 列表
来源：http://sx.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://td.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wj.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yo.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://no.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://eu.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://hr.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://mq.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wz.nszjky.cn

[D02] 追加元素到末尾
来源：http://ue.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wz.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wb.wgjwhj.cn

JS:   arr.push(4);
来源：http://ly.haigaiapp.cn

TS:   arr.push(4);
来源：http://ul.huanxung.cn

Java: list.add(4);
来源：http://gp.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://em.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://qo.lnxyls.cn

C#:   list.Add(4);
来源：http://mo.colortex.cn

[D03] 在指定位置插入元素
来源：http://pv.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://zh.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ra.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ln.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://id.hahajie.cn

Java: list.add(0, 0);
来源：http://jy.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lk.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nk.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://vb.shxzskj.cn

[D04] 删除元素
来源：http://zz.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xh.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ka.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mx.colortex.cn

TS:   arr.splice(0, 1);
来源：http://fn.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nv.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ow.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://or.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uu.hahajie.cn

[D05] 访问与修改元素
来源：http://lb.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pw.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jp.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ds.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://ig.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://ml.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://lx.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ul.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rf.nicolike.cn

[D06] 数组长度
来源：http://do.huanxung.cn

Py:   len(arr)
来源：http://cs.szxytkj.cn

PHP:  count($arr);
来源：http://jm.521024.cn

JS:   arr.length
来源：http://qb.hnjuh.cn

TS:   arr.length
来源：http://za.bookmarksfly.cn

Java: list.size();
来源：http://ee.muxihuayi.cn

Go:   len(arr)
来源：http://bk.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://uj.hnjuh.cn

C#:   list.Count;
来源：http://fg.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://ra.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rz.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ig.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://jf.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://tu.szsharing.cn

Java: list.subList(1, 4);
来源：http://ep.bjjhwx.cn

Go:   arr[1:4]
来源：http://pb.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://mr.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://no.bjjhwx.cn

[D08] 合并两个数组
来源：http://lh.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://is.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://qs.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hg.colortex.cn

TS:   [...a, ...b];
来源：http://vu.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://en.muxihuayi.cn

Go:   append(a, b...)
来源：http://de.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://cd.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://li.nszjky.cn

[D09] 排序（升序）
来源：http://ta.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://ch.shxzskj.cn

PHP:  sort($arr);
来源：http://aq.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bm.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ft.huanxung.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pb.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lt.huixiangedu.cn

Ruby: arr.sort
来源：http://tp.shxzskj.cn

C#:   list.Sort();
来源：http://bm.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tk.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kf.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fe.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fc.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uc.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tl.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ch.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ma.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hh.yuntaijiaju.cn

[D11] 反转数组
来源：http://et.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sf.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://gb.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://os.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://ce.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://lb.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://jr.bjjhwx.cn

Ruby: arr.reverse
来源：http://wh.muxihuayi.cn

C#:   list.Reverse();
来源：http://rm.nicolike.cn

[D12] 查找元素下标
来源：http://ws.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://un.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kz.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bf.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://er.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dq.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://fy.wgjwhj.cn

Ruby: arr.index(x)
来源：http://rh.nszjky.cn

C#:   list.IndexOf(x);
来源：http://me.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://ko.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ke.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hj.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://ry.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://ez.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xa.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lu.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tq.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mr.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://lc.haigaiapp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ow.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gp.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://fs.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://lg.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mv.jctech888.com.cn

Go:   // 手写循环
来源：http://lj.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ur.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ve.wgjwhj.cn

[D15] 去重
来源：http://ig.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wo.nicolike.cn

PHP:  array_unique($arr);
来源：http://bk.newstarts.cn

JS:   [...new Set(arr)]
来源：http://os.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://mc.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://on.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vi.hnjuh.cn

Ruby: arr.uniq
来源：http://qp.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://pc.gzmigu.cn

[D16] 求和与平均值
来源：http://wo.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bs.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iy.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ol.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://we.wgjwhj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kn.nszjky.cn

Go:   // 手写循环累加
来源：http://st.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lu.521024.cn

C#:   list.Sum();  list.Average()
来源：http://by.shxzskj.cn

[D17] 最大值与最小值
来源：http://xr.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://bu.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://jk.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pi.bookmarksfly.cn

TS:   Math.max(...arr);
来源：http://ja.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gj.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nm.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://vu.asd995.cn

C#:   list.Max();  list.Min()
来源：http://hh.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://qc.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cs.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://pp.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vf.521024.cn

TS:   nested.flat();
来源：http://px.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://js.jctech888.com.cn

Go:   // 手写双层循环
来源：http://sc.huixinmuqiang.cn

Ruby: nested.flatten
来源：http://nd.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jj.muxihuayi.cn

[D19] 按字段分组
来源：http://ou.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yv.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yo.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tb.lnxyls.cn


<!-- 参考信息 -->