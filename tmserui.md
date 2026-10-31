代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://dm.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nw.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://xr.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wp.muxihuayi.cn

[C02] 默认参数
来源：http://my.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://ot.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bd.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://cj.huixinmuqiang.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vy.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://eq.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hx.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://qn.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://ek.szsharing.cn

[C03] 可变参数
来源：http://hz.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://qd.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bf.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zs.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cy.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xn.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kd.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fm.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fr.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://yd.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xk.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://op.hnjuh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fk.panjiajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ld.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://ch.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://az.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://ag.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://tw.lnxyls.cn

[C05] 返回多个值
来源：http://cx.chemitech.net.cn

Py:   return a, b
来源：http://mr.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://pq.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jd.szxytkj.cn

TS:   return { a, b };
来源：http://le.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vy.shtwfgs.cn

Go:   return a, b
来源：http://gm.asd995.cn

Ruby: return a, b
来源：http://ji.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://sr.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://sv.nicolike.cn

Py:   square = lambda x: x * x
来源：http://tz.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://te.hnjuh.cn

JS:   const square = x => x * x;
来源：http://jn.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://jd.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kz.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://va.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://wi.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://my.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://ct.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kf.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yq.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://py.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://en.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pi.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xa.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://jw.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://og.shxzukj.cn

[C08] 闭包
来源：http://be.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tt.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hl.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uy.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ad.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ki.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ap.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uk.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rd.jctech888.com.cn

[C09] 递归
来源：http://ri.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lb.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ea.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fk.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zs.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gk.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zc.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nm.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ns.newstarts.cn

[C10] 变量作用域
来源：http://rt.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lp.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jp.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vp.szsharing.cn

TS:   同 JS
来源：http://jd.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://rm.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://wz.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lc.yuntaijiaju.cn

C#:   块级作用域
来源：http://rj.shxzukj.cn

[C11] 模块导入与导出
来源：http://cm.asd995.cn

Py:   from module import func
来源：http://tu.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://oc.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pu.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zg.muxihuayi.cn

Java: import java.util.List;
来源：http://wk.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xy.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://ug.chemitech.net.cn

C#:   using System.Text;
来源：http://pp.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://lj.asd995.cn

Py:   (lambda: print("run"))()
来源：http://lv.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://nf.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://ny.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://nv.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ym.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://hc.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://hi.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ve.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://ji.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wa.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tt.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fw.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://or.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sl.asd995.cn

Go:   func add(a, b int) int
来源：http://tv.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lh.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://iv.bookmarksfly.cn

[C14] 泛型函数
来源：http://aw.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dn.hahajie.cn

PHP:  // 无泛型
来源：http://zj.newstarts.cn

JS:   // 无泛型
来源：http://yb.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cb.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uh.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zf.lnxyls.cn

Ruby: # 无泛型
来源：http://mx.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hx.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://mb.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vr.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://ao.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wy.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vf.gzmigu.cn

Java: // 无解构
来源：http://wx.bjjhwx.cn

Go:   // 无解构
来源：http://pg.huixiangedu.cn

Ruby: a, b = pair
来源：http://gu.hahajie.cn

C#:   var (a, b) = pair;
来源：http://uw.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://wr.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qb.szsharing.cn

PHP:  // 无重载
来源：http://na.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lk.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://rr.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rl.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://ov.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://gw.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://or.gzmigu.cn

================================================================================
来源：http://vm.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://jx.szxytkj.cn

================================================================================
来源：http://yi.nicolike.cn

[D01] 创建数组 / 列表
来源：http://yj.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fy.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cx.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pz.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nq.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dx.shtwfgs.cn

Go:   arr := []int{1, 2, 3}
来源：http://eb.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://jg.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dk.hahajie.cn

[D02] 追加元素到末尾
来源：http://rq.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://am.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kg.521024.cn

JS:   arr.push(4);
来源：http://ht.huanxung.cn

TS:   arr.push(4);
来源：http://xy.haigaiapp.cn

Java: list.add(4);
来源：http://ig.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://vu.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://nf.bjjhwx.cn

C#:   list.Add(4);
来源：http://ps.huanxung.cn

[D03] 在指定位置插入元素
来源：http://oo.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://tj.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dr.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mm.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://tq.wgjwhj.cn

Java: list.add(0, 0);
来源：http://rj.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ej.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://je.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://qj.szxytkj.cn

[D04] 删除元素
来源：http://wh.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ft.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tn.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nz.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://ih.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oi.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cx.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nn.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dl.nicolike.cn

[D05] 访问与修改元素
来源：http://am.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ce.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rz.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vj.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://gm.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://xd.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://dm.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://co.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eu.shtwfgs.cn

[D06] 数组长度
来源：http://dg.huixinmuqiang.cn

Py:   len(arr)
来源：http://hp.nszjky.cn

PHP:  count($arr);
来源：http://ln.szsharing.cn

JS:   arr.length
来源：http://fs.521024.cn

TS:   arr.length
来源：http://bh.muxihuayi.cn

Java: list.size();
来源：http://kb.hahajie.cn

Go:   len(arr)
来源：http://qb.colortex.cn

Ruby: arr.length; arr.size
来源：http://wg.nicolike.cn

C#:   list.Count;
来源：http://zr.nszjky.cn

[D07] 切片 / 取子数组
来源：http://sr.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qy.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://aj.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://ua.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://tb.shxzskj.cn

Java: list.subList(1, 4);
来源：http://ib.shxzskj.cn

Go:   arr[1:4]
来源：http://ko.nicolike.cn

Ruby: arr[1, 3]
来源：http://iu.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://wa.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://qf.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://gn.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://xe.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xx.nicolike.cn

TS:   [...a, ...b];
来源：http://ts.521024.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gm.hnjuh.cn

Go:   append(a, b...)
来源：http://ay.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://ps.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://re.huixiangedu.cn

[D09] 排序（升序）
来源：http://nt.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://ki.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://pl.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://va.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bq.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://eb.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://az.huixiangedu.cn

Ruby: arr.sort
来源：http://px.huanxung.cn

C#:   list.Sort();
来源：http://bp.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iz.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rc.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nc.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sc.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uc.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mp.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ha.shtwfgs.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tg.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ne.yuntaijiaju.cn

[D11] 反转数组
来源：http://dj.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lq.szsharing.cn

PHP:  array_reverse($arr);
来源：http://hl.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ju.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://xk.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://xz.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://lx.shxzukj.cn

Ruby: arr.reverse
来源：http://qb.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://cx.colortex.cn

[D12] 查找元素下标
来源：http://yx.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://jz.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gi.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ot.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ob.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ss.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://nq.huixiangedu.cn

Ruby: arr.index(x)
来源：http://nx.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://qr.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://wj.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://br.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jx.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://wt.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://td.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gy.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ub.shxzukj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uw.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gs.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://xc.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ol.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ge.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://gr.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://gn.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pq.521024.cn

Go:   // 手写循环
来源：http://uz.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dd.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sn.huixinmuqiang.cn

[D15] 去重
来源：http://gt.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wk.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://is.9csxet.cn

JS:   [...new Set(arr)]
来源：http://ty.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://pr.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vu.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://te.shxzukj.cn

Ruby: arr.uniq
来源：http://hw.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://ps.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://xo.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://al.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jd.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bi.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bf.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ga.shtwfgs.cn

Go:   // 手写循环累加
来源：http://og.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qh.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://db.9csxet.cn

[D17] 最大值与最小值
来源：http://ky.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://fx.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://mh.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qg.gzmigu.cn

TS:   Math.max(...arr);
来源：http://xc.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://if.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hj.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://bz.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://vs.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://oo.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gc.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://xa.9csxet.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hm.nicolike.cn

TS:   nested.flat();
来源：http://ff.huixiangedu.cn


<!-- 参考信息 -->