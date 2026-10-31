代发 wailian999

[C02] 默认参数
来源：http://fb.colortex.cn

Py:   def greet(name="World"): return name
来源：http://qp.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qk.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://xo.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://th.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gj.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jq.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://vx.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://vp.chemitech.net.cn

[C03] 可变参数
来源：http://uf.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://av.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ej.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jq.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ei.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pr.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ab.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://js.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hc.shxzukj.cn

[C04] 命名参数 / 关键字参数
来源：http://nn.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qk.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sg.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ml.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gs.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://kp.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://xc.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://xb.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://xl.huanxung.cn

[C05] 返回多个值
来源：http://ax.nicolike.cn

Py:   return a, b
来源：http://yx.521024.cn

PHP:  return [$a, $b];
来源：http://fh.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bx.panjiajie.cn

TS:   return { a, b };
来源：http://br.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ba.jctech888.com.cn

Go:   return a, b
来源：http://kj.hahajie.cn

Ruby: return a, b
来源：http://aj.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://xy.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://xm.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://xg.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vv.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://sw.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://cy.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hd.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zx.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://om.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cg.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://cy.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pl.yuexingan06.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fz.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://es.wgjwhj.cn

TS:   arr.map(String)
来源：http://ax.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pb.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ni.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://ra.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://po.colortex.cn

[C08] 闭包
来源：http://bj.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mz.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xc.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yr.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kt.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lo.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jq.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nw.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dw.jctech888.com.cn

[C09] 递归
来源：http://kq.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vl.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oh.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rv.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://et.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xm.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jk.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://os.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zi.shtwfgs.cn

[C10] 变量作用域
来源：http://tp.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ha.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://or.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vi.huanxung.cn

TS:   同 JS
来源：http://fq.lnxyls.cn

Java: 方法内为块级作用域
来源：http://dc.huanxung.cn

Go:   花括号块级作用域
来源：http://kn.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ov.chemitech.net.cn

C#:   块级作用域
来源：http://dq.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://oc.nicolike.cn

Py:   from module import func
来源：http://yh.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ey.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ya.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bp.shtwfgs.cn

Java: import java.util.List;
来源：http://ex.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dx.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://dl.521024.cn

C#:   using System.Text;
来源：http://lc.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://tg.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://da.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://xi.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://vo.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://le.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tf.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://jm.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://nr.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sf.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://yb.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://om.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fe.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://su.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nc.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ss.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://sl.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mf.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bb.haigaiapp.cn

[C14] 泛型函数
来源：http://jh.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qa.huanxung.cn

PHP:  // 无泛型
来源：http://iz.muxihuayi.cn

JS:   // 无泛型
来源：http://dj.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mx.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wn.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oz.szxytkj.cn

Ruby: # 无泛型
来源：http://ma.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tl.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://cs.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yo.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://lj.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gw.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ww.nszjky.cn

Java: // 无解构
来源：http://ia.gzmigu.cn

Go:   // 无解构
来源：http://uk.shtwfgs.cn

Ruby: a, b = pair
来源：http://fw.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://ns.521024.cn

[C16] 函数 / 方法重载
来源：http://qm.colortex.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tt.szxytkj.cn

PHP:  // 无重载
来源：http://xp.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qg.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://fv.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fc.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://ve.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://ue.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ax.nicolike.cn

================================================================================
来源：http://mc.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://cz.yuntaijiaju.cn

================================================================================
来源：http://ea.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://xc.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vx.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ye.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zz.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ux.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rk.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://zg.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://cx.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jp.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://vy.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ot.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gg.9csxet.cn

JS:   arr.push(4);
来源：http://dk.huanxung.cn

TS:   arr.push(4);
来源：http://yp.gzmigu.cn

Java: list.add(4);
来源：http://tt.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://sl.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://mb.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://bt.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://sk.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://as.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fo.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bz.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://yb.hahajie.cn

Java: list.add(0, 0);
来源：http://ot.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ij.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pp.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://zc.asd995.cn

[D04] 删除元素
来源：http://dw.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jl.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tu.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qf.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://sy.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ga.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zx.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mm.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zg.jctech888.com.cn

[D05] 访问与修改元素
来源：http://wn.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nu.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jn.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ou.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://bo.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://cr.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://sb.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vs.muxihuayi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ls.szxytkj.cn

[D06] 数组长度
来源：http://nv.hnjuh.cn

Py:   len(arr)
来源：http://yh.shxzukj.cn

PHP:  count($arr);
来源：http://ig.wgjwhj.cn

JS:   arr.length
来源：http://co.huixinmuqiang.cn

TS:   arr.length
来源：http://zi.gzmigu.cn

Java: list.size();
来源：http://bw.shtwfgs.cn

Go:   len(arr)
来源：http://qp.asd995.cn

Ruby: arr.length; arr.size
来源：http://bt.chemitech.net.cn

C#:   list.Count;
来源：http://fm.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://qu.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pf.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tp.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://hb.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://fy.huanxung.cn

Java: list.subList(1, 4);
来源：http://jq.asd995.cn

Go:   arr[1:4]
来源：http://mp.shxzukj.cn

Ruby: arr[1, 3]
来源：http://sc.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://pb.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://xh.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://st.colortex.cn

PHP:  array_merge($a, $b);
来源：http://tt.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pz.521024.cn

TS:   [...a, ...b];
来源：http://sg.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ir.haigaiapp.cn

Go:   append(a, b...)
来源：http://wb.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://cu.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://al.yuexingan06.cn

[D09] 排序（升序）
来源：http://vh.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://fs.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://se.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ll.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xz.nicolike.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fd.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bk.gzmigu.cn

Ruby: arr.sort
来源：http://zr.9csxet.cn

C#:   list.Sort();
来源：http://dd.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ry.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iw.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yz.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ys.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ju.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cp.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xz.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ax.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ja.bookmarksfly.cn

[D11] 反转数组
来源：http://xo.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tj.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://su.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kk.huixinmuqiang.cn

TS:   [...arr].reverse();
来源：http://me.shxzukj.cn

Java: Collections.reverse(list);
来源：http://mq.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://zk.shxzskj.cn

Ruby: arr.reverse
来源：http://xk.gzmigu.cn

C#:   list.Reverse();
来源：http://ui.wgjwhj.cn

[D12] 查找元素下标
来源：http://ld.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://sa.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ps.huanxung.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vu.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jp.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bs.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://te.521024.cn

Ruby: arr.index(x)
来源：http://hj.hahajie.cn

C#:   list.IndexOf(x);
来源：http://gm.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://zt.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ce.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dq.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://be.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://kq.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uz.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gu.shxzukj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fq.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://om.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://si.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://br.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ak.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://zf.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://nv.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ls.colortex.cn

Go:   // 手写循环
来源：http://do.muxihuayi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nr.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cz.yuexingan06.cn

[D15] 去重
来源：http://ps.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sb.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://mq.hahajie.cn

JS:   [...new Set(arr)]
来源：http://ko.nicolike.cn

TS:   [...new Set(arr)]
来源：http://tr.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ll.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://om.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://uu.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://yg.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://ta.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fo.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bl.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ux.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ku.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eb.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://kq.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ns.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://kw.asd995.cn

[D17] 最大值与最小值
来源：http://vw.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://mh.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://ax.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gz.hnjuh.cn

TS:   Math.max(...arr);
来源：http://pd.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jk.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kn.colortex.cn

Ruby: arr.max;  arr.min
来源：http://hy.asd995.cn

C#:   list.Max();  list.Min()
来源：http://in.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://jg.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qx.521024.cn

PHP:  array_merge(...$nested);
来源：http://nj.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nw.hahajie.cn

TS:   nested.flat();
来源：http://bk.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sb.bjjhwx.cn

Go:   // 手写双层循环
来源：http://pg.bookmarksfly.cn

Ruby: nested.flatten
来源：http://tk.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://va.muxihuayi.cn


<!-- 参考信息 -->