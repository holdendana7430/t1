代发 wailian999

Py:   def add(a, b): return a + b
来源：http://ul.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://di.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://wr.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ar.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pa.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jp.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://mr.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kf.panjiajie.cn

[C02] 默认参数
来源：http://rw.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://ll.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tv.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://mm.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hh.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gj.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://du.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://mo.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://ym.jianghongdianzi.cn

[C03] 可变参数
来源：http://wg.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://bp.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yj.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dv.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gn.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hj.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rb.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yf.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jt.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://fi.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lu.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oh.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rx.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fb.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://xg.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://zx.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://na.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://mw.asd995.cn

[C05] 返回多个值
来源：http://uz.yuexingan06.cn

Py:   return a, b
来源：http://cr.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://xw.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hu.wgjwhj.cn

TS:   return { a, b };
来源：http://ht.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vm.bjjhwx.cn

Go:   return a, b
来源：http://mn.nicolike.cn

Ruby: return a, b
来源：http://pb.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://ho.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://lm.newstarts.cn

Py:   square = lambda x: x * x
来源：http://uk.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bz.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://gw.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://jg.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gu.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vq.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://fb.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xs.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://dx.bookmarksfly.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bx.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ma.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tn.9csxet.cn

TS:   arr.map(String)
来源：http://ma.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lk.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qh.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://cp.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bj.nicolike.cn

[C08] 闭包
来源：http://kb.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qi.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uv.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dm.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nk.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dy.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gb.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xx.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lb.jianghongdianzi.cn

[C09] 递归
来源：http://yx.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aq.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://po.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://su.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jb.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xi.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vd.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hp.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tl.huixiangedu.cn

[C10] 变量作用域
来源：http://su.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ju.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zs.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hh.jctech888.com.cn

TS:   同 JS
来源：http://gp.nicolike.cn

Java: 方法内为块级作用域
来源：http://sf.szsharing.cn

Go:   花括号块级作用域
来源：http://uw.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hb.panjiajie.cn

C#:   块级作用域
来源：http://ub.shtwfgs.cn

[C11] 模块导入与导出
来源：http://bn.shtwfgs.cn

Py:   from module import func
来源：http://dt.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kl.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://un.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yd.wgjwhj.cn

Java: import java.util.List;
来源：http://vb.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fm.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://sw.yuntaijiaju.cn

C#:   using System.Text;
来源：http://ob.521024.cn

[C12] 立即执行函数 IIFE
来源：http://yf.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://ol.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://pw.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://pa.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://wx.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vf.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://pf.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://rs.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nv.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://xk.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gw.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qm.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uc.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ab.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ib.szxytkj.cn

Go:   func add(a, b int) int
来源：http://vw.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eq.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zu.jianghongdianzi.cn

[C14] 泛型函数
来源：http://dp.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tq.muxihuayi.cn

PHP:  // 无泛型
来源：http://qt.bjjhwx.cn

JS:   // 无泛型
来源：http://do.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gk.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://di.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://my.panjiajie.cn

Ruby: # 无泛型
来源：http://as.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lu.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://em.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eq.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://hv.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hq.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mr.szxytkj.cn

Java: // 无解构
来源：http://sk.jianghongdianzi.cn

Go:   // 无解构
来源：http://ad.asd995.cn

Ruby: a, b = pair
来源：http://qi.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://qp.asd995.cn

[C16] 函数 / 方法重载
来源：http://qg.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vc.lnxyls.cn

PHP:  // 无重载
来源：http://up.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://iv.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://sf.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gb.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://vd.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://bi.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gp.9csxet.cn

================================================================================
来源：http://dz.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://qe.huixinmuqiang.cn

================================================================================
来源：http://bq.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://yw.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://on.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ql.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yy.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gl.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ws.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://uy.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://zj.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://do.gzmigu.cn

[D02] 追加元素到末尾
来源：http://ds.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zz.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qa.panjiajie.cn

JS:   arr.push(4);
来源：http://ck.colortex.cn

TS:   arr.push(4);
来源：http://gw.muxihuayi.cn

Java: list.add(4);
来源：http://gy.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://dv.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://xr.szsharing.cn

C#:   list.Add(4);
来源：http://fy.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://ba.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://yz.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ax.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ox.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ot.panjiajie.cn

Java: list.add(0, 0);
来源：http://fg.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fh.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wc.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://xw.szxytkj.cn

[D04] 删除元素
来源：http://aw.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kj.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eh.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bq.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://xn.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ce.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ti.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qa.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lu.szsharing.cn

[D05] 访问与修改元素
来源：http://qt.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xv.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ys.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uv.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://es.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://ry.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://zd.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oh.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wr.nicolike.cn

[D06] 数组长度
来源：http://ib.shxzskj.cn

Py:   len(arr)
来源：http://ai.szsharing.cn

PHP:  count($arr);
来源：http://ij.shtwfgs.cn

JS:   arr.length
来源：http://us.bookmarksfly.cn

TS:   arr.length
来源：http://xz.lnxyls.cn

Java: list.size();
来源：http://rl.nszjky.cn

Go:   len(arr)
来源：http://sm.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://db.jctech888.com.cn

C#:   list.Count;
来源：http://ui.nszjky.cn

[D07] 切片 / 取子数组
来源：http://yg.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kf.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://an.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://qv.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://mc.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://sn.nszjky.cn

Go:   arr[1:4]
来源：http://us.nszjky.cn

Ruby: arr[1, 3]
来源：http://bo.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://iy.yuexingan06.cn

[D08] 合并两个数组
来源：http://gi.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://om.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://sw.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hg.muxihuayi.cn

TS:   [...a, ...b];
来源：http://kj.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ic.521024.cn

Go:   append(a, b...)
来源：http://az.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://ew.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://pd.panjiajie.cn

[D09] 排序（升序）
来源：http://ua.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://if.szxytkj.cn

PHP:  sort($arr);
来源：http://zb.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ie.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oz.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tb.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jr.lnxyls.cn

Ruby: arr.sort
来源：http://sa.shxzskj.cn

C#:   list.Sort();
来源：http://tr.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ik.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ef.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rk.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bc.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fm.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dy.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ei.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nx.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mk.shxzukj.cn

[D11] 反转数组
来源：http://qz.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nw.nszjky.cn

PHP:  array_reverse($arr);
来源：http://pt.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://da.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://un.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://hh.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://cp.bjjhwx.cn

Ruby: arr.reverse
来源：http://ml.shxzskj.cn

C#:   list.Reverse();
来源：http://sq.colortex.cn

[D12] 查找元素下标
来源：http://bm.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://bm.newstarts.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://un.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lf.shtwfgs.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rj.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wt.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://pe.chemitech.net.cn

Ruby: arr.index(x)
来源：http://ur.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://uz.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://jr.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://da.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ka.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://ge.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://qs.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cc.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lu.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tu.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jq.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://kn.521024.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dr.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oz.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://qe.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://mc.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mi.9csxet.cn

Go:   // 手写循环
来源：http://rz.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zp.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://db.szxytkj.cn

[D15] 去重
来源：http://ca.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://td.colortex.cn

PHP:  array_unique($arr);
来源：http://fs.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://vj.gzmigu.cn

TS:   [...new Set(arr)]
来源：http://qp.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fz.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nc.lnxyls.cn

Ruby: arr.uniq
来源：http://qr.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://xg.haigaiapp.cn

[D16] 求和与平均值
来源：http://ml.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uj.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zs.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mu.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vb.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zm.colortex.cn

Go:   // 手写循环累加
来源：http://pm.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ze.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://ky.hnjuh.cn

[D17] 最大值与最小值
来源：http://hd.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://bs.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://yo.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jc.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://lc.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gm.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wh.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://ry.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://xl.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://yz.huixinmuqiang.cn


<!-- 参考信息 -->