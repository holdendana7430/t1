代发 wailian999

Py:   if not data: return
来源：http://rl.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://zy.shxzukj.cn

JS:   if (!data) return;
来源：http://xo.gzmigu.cn

TS:   if (!data) return;
来源：http://tr.huanxung.cn

Java: if (data == null) return;
来源：http://ck.nszjky.cn

Go:   if data == nil { return }
来源：http://fo.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://ed.hahajie.cn

C#:   if (data == null) return;
来源：http://ud.huixinmuqiang.cn

================================================================================
来源：http://ez.bookmarksfly.cn

C. 函数与作用域
来源：http://ac.gzmigu.cn

================================================================================
来源：http://xo.nicolike.cn

[C01] 定义函数
来源：http://rl.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://bl.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gv.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://ox.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rl.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cg.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qy.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://rh.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://js.chemitech.net.cn

[C02] 默认参数
来源：http://ax.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://rx.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jw.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://yb.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lx.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ql.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fi.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://yq.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://mm.nicolike.cn

[C03] 可变参数
来源：http://xi.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://eh.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yd.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xh.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yl.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://li.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://td.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tp.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oc.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://tt.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mi.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tg.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zz.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ij.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://or.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://yp.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://pa.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://we.huixinmuqiang.cn

[C05] 返回多个值
来源：http://sh.lnxyls.cn

Py:   return a, b
来源：http://dc.gzmigu.cn

PHP:  return [$a, $b];
来源：http://rn.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xg.gzmigu.cn

TS:   return { a, b };
来源：http://wm.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lk.lnxyls.cn

Go:   return a, b
来源：http://id.newstarts.cn

Ruby: return a, b
来源：http://fj.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://rv.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://rs.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://aq.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vg.szsharing.cn

JS:   const square = x => x * x;
来源：http://az.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://ix.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fq.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://en.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://cl.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://au.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://zd.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ji.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nl.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yk.nicolike.cn

TS:   arr.map(String)
来源：http://fo.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bt.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yq.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://hm.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sm.9csxet.cn

[C08] 闭包
来源：http://yi.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ap.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rx.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vt.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bv.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vs.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pj.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cj.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pg.shtwfgs.cn

[C09] 递归
来源：http://fj.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dj.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ei.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nr.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sa.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wx.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ak.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://et.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yh.521024.cn

[C10] 变量作用域
来源：http://dg.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ll.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wh.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://im.hnjuh.cn

TS:   同 JS
来源：http://rc.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://np.wgjwhj.cn

Go:   花括号块级作用域
来源：http://la.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nz.gzmigu.cn

C#:   块级作用域
来源：http://up.chemitech.net.cn

[C11] 模块导入与导出
来源：http://hh.wgjwhj.cn

Py:   from module import func
来源：http://gn.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ex.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://et.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wn.haigaiapp.cn

Java: import java.util.List;
来源：http://wx.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bl.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://fu.521024.cn

C#:   using System.Text;
来源：http://ax.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://xc.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://vg.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://ua.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://jk.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://jh.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rw.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://ds.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://wq.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jy.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://bb.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gb.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ay.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ty.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rj.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gi.asd995.cn

Go:   func add(a, b int) int
来源：http://yv.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lp.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://le.huanxung.cn

[C14] 泛型函数
来源：http://rx.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tn.asd995.cn

PHP:  // 无泛型
来源：http://kc.lnxyls.cn

JS:   // 无泛型
来源：http://zg.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ax.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://re.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kt.hahajie.cn

Ruby: # 无泛型
来源：http://sr.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nu.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://ql.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wn.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://fz.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://py.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gk.yuntaijiaju.cn

Java: // 无解构
来源：http://ol.nszjky.cn

Go:   // 无解构
来源：http://py.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://uz.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://ib.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://um.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cu.chemitech.net.cn

PHP:  // 无重载
来源：http://dt.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qw.huixinmuqiang.cn

TS:   // 用联合类型或重载签名声明
来源：http://an.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://db.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://mf.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://pt.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://of.bjjhwx.cn

================================================================================
来源：http://eg.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://iz.521024.cn

================================================================================
来源：http://wq.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://tw.521024.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bv.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ii.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yd.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qd.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oj.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://el.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://va.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://of.nicolike.cn

[D02] 追加元素到末尾
来源：http://ad.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ms.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wp.shxzukj.cn

JS:   arr.push(4);
来源：http://pn.shxzskj.cn

TS:   arr.push(4);
来源：http://tt.bookmarksfly.cn

Java: list.add(4);
来源：http://ys.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://sn.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://ry.panjiajie.cn

C#:   list.Add(4);
来源：http://kj.nicolike.cn

[D03] 在指定位置插入元素
来源：http://nw.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://ml.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ro.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://or.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://im.asd995.cn

Java: list.add(0, 0);
来源：http://bb.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xr.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tf.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://wh.newstarts.cn

[D04] 删除元素
来源：http://uj.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ck.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tb.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qm.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://ug.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cl.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ki.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jp.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rw.asd995.cn

[D05] 访问与修改元素
来源：http://rc.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://aq.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ms.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sk.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://du.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://zy.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://rq.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ms.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aq.lnxyls.cn

[D06] 数组长度
来源：http://va.bjjhwx.cn

Py:   len(arr)
来源：http://dc.gzmigu.cn

PHP:  count($arr);
来源：http://br.szxytkj.cn

JS:   arr.length
来源：http://oa.szsharing.cn

TS:   arr.length
来源：http://oz.gzmigu.cn

Java: list.size();
来源：http://lz.colortex.cn

Go:   len(arr)
来源：http://lp.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://ek.newstarts.cn

C#:   list.Count;
来源：http://al.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://at.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vv.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gl.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://xf.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://wm.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://rx.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://fe.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://zi.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://wm.nicolike.cn

[D08] 合并两个数组
来源：http://ac.521024.cn

Py:   a + b;  a.extend(b)
来源：http://an.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://ew.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dv.szsharing.cn

TS:   [...a, ...b];
来源：http://rl.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://si.hnjuh.cn

Go:   append(a, b...)
来源：http://jp.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://xy.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://nm.colortex.cn

[D09] 排序（升序）
来源：http://fx.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://av.bookmarksfly.cn

PHP:  sort($arr);
来源：http://av.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zx.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zx.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vb.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wf.hnjuh.cn

Ruby: arr.sort
来源：http://bg.huanxung.cn

C#:   list.Sort();
来源：http://et.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vh.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lf.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bn.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ww.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oi.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ub.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yy.colortex.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oc.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pu.szxytkj.cn

[D11] 反转数组
来源：http://bc.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tz.hahajie.cn

PHP:  array_reverse($arr);
来源：http://fk.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ao.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://qg.gzmigu.cn

Java: Collections.reverse(list);
来源：http://ty.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://nd.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://xk.szsharing.cn

C#:   list.Reverse();
来源：http://fi.nicolike.cn

[D12] 查找元素下标
来源：http://qi.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://un.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zh.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hl.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nm.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iv.colortex.cn

Go:   slices.Index(arr, x)
来源：http://kl.yuexingan06.cn

Ruby: arr.index(x)
来源：http://ym.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://gz.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://jv.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cf.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ch.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://ee.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://xy.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lp.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ff.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ww.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://aw.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://qg.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cg.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://to.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://jx.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://vo.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://de.lnxyls.cn

Go:   // 手写循环
来源：http://ri.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kw.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gy.yuntaijiaju.cn

[D15] 去重
来源：http://oq.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cc.newstarts.cn

PHP:  array_unique($arr);
来源：http://vp.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://op.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://np.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ef.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://up.newstarts.cn

Ruby: arr.uniq
来源：http://nx.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://sx.nicolike.cn

[D16] 求和与平均值
来源：http://oy.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gc.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iu.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zc.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zc.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tl.lnxyls.cn

Go:   // 手写循环累加
来源：http://hb.hnjuh.cn


<!-- 参考信息 -->