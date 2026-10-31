代发 wailian999

Java: if (data == null) return;
来源：http://lf.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://ox.9csxet.cn

Ruby: return if data.nil?
来源：http://fg.521024.cn

C#:   if (data == null) return;
来源：http://hz.panjiajie.cn

================================================================================
来源：http://zk.shxzukj.cn

C. 函数与作用域
来源：http://kc.szxytkj.cn

================================================================================
来源：http://ao.yuexingan06.cn

[C01] 定义函数
来源：http://zg.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://oh.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pt.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://gh.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ut.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pa.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ce.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://rg.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wz.lnxyls.cn

[C02] 默认参数
来源：http://yx.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://bc.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tt.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://ev.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yq.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bq.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gt.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://nn.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://eq.jianghongdianzi.cn

[C03] 可变参数
来源：http://hz.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://jh.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sp.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wz.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lr.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jb.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ff.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tp.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sb.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://io.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yd.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ae.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xf.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uf.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://bk.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://lg.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://uj.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://cd.haigaiapp.cn

[C05] 返回多个值
来源：http://bl.nicolike.cn

Py:   return a, b
来源：http://fy.newstarts.cn

PHP:  return [$a, $b];
来源：http://es.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ak.lnxyls.cn

TS:   return { a, b };
来源：http://xh.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jw.yuntaijiaju.cn

Go:   return a, b
来源：http://op.huixinmuqiang.cn

Ruby: return a, b
来源：http://cn.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://bq.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://iq.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://xm.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kd.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://sw.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ql.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bv.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wa.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://ne.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pt.szsharing.cn

[C07] 把函数作为参数传入
来源：http://fs.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jp.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fr.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bs.shxzskj.cn

TS:   arr.map(String)
来源：http://xh.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ys.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uc.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://py.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xl.521024.cn

[C08] 闭包
来源：http://qu.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ku.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qo.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://er.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tg.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fx.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jt.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jl.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ba.hnjuh.cn

[C09] 递归
来源：http://ey.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wi.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://br.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nk.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://de.chemitech.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sl.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zl.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dz.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://po.gzmigu.cn

[C10] 变量作用域
来源：http://ag.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gn.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hh.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eu.muxihuayi.cn

TS:   同 JS
来源：http://ca.szsharing.cn

Java: 方法内为块级作用域
来源：http://ai.shxzskj.cn

Go:   花括号块级作用域
来源：http://nn.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hn.nszjky.cn

C#:   块级作用域
来源：http://bl.huixiangedu.cn

[C11] 模块导入与导出
来源：http://xn.gzmigu.cn

Py:   from module import func
来源：http://de.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rr.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cx.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bd.shtwfgs.cn

Java: import java.util.List;
来源：http://ry.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://go.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://pv.9csxet.cn

C#:   using System.Text;
来源：http://gw.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://td.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://vd.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://am.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://ah.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://zy.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cl.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://mb.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://lk.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nt.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://sa.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nw.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cc.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://la.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cw.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nl.shxzskj.cn

Go:   func add(a, b int) int
来源：http://wo.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xv.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dk.gzmigu.cn

[C14] 泛型函数
来源：http://ot.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lr.lnxyls.cn

PHP:  // 无泛型
来源：http://eu.asd995.cn

JS:   // 无泛型
来源：http://qv.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xs.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bg.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ec.bjjhwx.cn

Ruby: # 无泛型
来源：http://io.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://of.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://fu.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xq.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://ya.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cf.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yt.haigaiapp.cn

Java: // 无解构
来源：http://xe.hahajie.cn

Go:   // 无解构
来源：http://ro.haigaiapp.cn

Ruby: a, b = pair
来源：http://yy.huanxung.cn

C#:   var (a, b) = pair;
来源：http://ig.newstarts.cn

[C16] 函数 / 方法重载
来源：http://fk.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ha.nszjky.cn

PHP:  // 无重载
来源：http://vh.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fh.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://tg.panjiajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xz.szxytkj.cn

Go:   // 无重载：用不同函数名
来源：http://kq.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://hh.shxzukj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mk.9csxet.cn

================================================================================
来源：http://np.colortex.cn

D. 数组 / 列表 / 集合
来源：http://dn.panjiajie.cn

================================================================================
来源：http://lv.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://ru.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ql.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ru.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yf.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://io.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ip.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://ap.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://cd.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uo.hnjuh.cn

[D02] 追加元素到末尾
来源：http://wo.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jm.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qj.szsharing.cn

JS:   arr.push(4);
来源：http://me.newstarts.cn

TS:   arr.push(4);
来源：http://wk.szsharing.cn

Java: list.add(4);
来源：http://yx.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://bt.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://mc.colortex.cn

C#:   list.Add(4);
来源：http://oo.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://ws.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://bx.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sz.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ig.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://kt.shxzukj.cn

Java: list.add(0, 0);
来源：http://ny.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wx.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fd.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://ys.wgjwhj.cn

[D04] 删除元素
来源：http://lx.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tb.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hd.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pi.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://si.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ox.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yv.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sn.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ct.panjiajie.cn

[D05] 访问与修改元素
来源：http://uh.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qk.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cq.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://de.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://iy.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://ar.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://wf.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ar.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hi.huixinmuqiang.cn

[D06] 数组长度
来源：http://ny.shtwfgs.cn

Py:   len(arr)
来源：http://fu.colortex.cn

PHP:  count($arr);
来源：http://ga.huixiangedu.cn

JS:   arr.length
来源：http://og.huixiangedu.cn

TS:   arr.length
来源：http://vs.shxzukj.cn

Java: list.size();
来源：http://ib.chemitech.net.cn

Go:   len(arr)
来源：http://uz.nszjky.cn

Ruby: arr.length; arr.size
来源：http://eu.yuexingan06.cn

C#:   list.Count;
来源：http://xu.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://xp.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sq.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qq.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://ag.shtwfgs.cn

TS:   arr.slice(1, 4);
来源：http://oj.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://kg.yuexingan06.cn

Go:   arr[1:4]
来源：http://dx.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://fg.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://ig.nicolike.cn

[D08] 合并两个数组
来源：http://mq.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://bm.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://ad.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://az.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://jb.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jd.jctech888.com.cn

Go:   append(a, b...)
来源：http://tg.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://gg.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://gv.nicolike.cn

[D09] 排序（升序）
来源：http://tf.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://bw.newstarts.cn

PHP:  sort($arr);
来源：http://mw.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://em.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ch.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ao.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kl.muxihuayi.cn

Ruby: arr.sort
来源：http://xu.shxzukj.cn

C#:   list.Sort();
来源：http://md.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bf.9csxet.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://in.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qy.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ul.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ja.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ul.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dk.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gu.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hs.huanxung.cn

[D11] 反转数组
来源：http://gn.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ol.asd995.cn

PHP:  array_reverse($arr);
来源：http://mg.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ng.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://wn.521024.cn

Java: Collections.reverse(list);
来源：http://mk.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://hq.szsharing.cn

Ruby: arr.reverse
来源：http://dg.muxihuayi.cn

C#:   list.Reverse();
来源：http://im.huanxung.cn

[D12] 查找元素下标
来源：http://gr.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://cu.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fy.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://we.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nj.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wa.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://zb.gzmigu.cn

Ruby: arr.index(x)
来源：http://fy.hahajie.cn

C#:   list.IndexOf(x);
来源：http://xb.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://le.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://he.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ty.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://sh.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://ve.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yz.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jz.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rw.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vv.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://sn.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kh.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ns.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://nf.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://ze.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zb.hahajie.cn

Go:   // 手写循环
来源：http://zt.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cl.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nx.panjiajie.cn

[D15] 去重
来源：http://nz.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ls.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://cs.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://ls.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://au.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fy.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://un.muxihuayi.cn

Ruby: arr.uniq
来源：http://pf.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://iz.bjjhwx.cn

[D16] 求和与平均值
来源：http://gi.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zv.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ce.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yg.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yu.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gg.newstarts.cn

Go:   // 手写循环累加
来源：http://kc.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ge.521024.cn

C#:   list.Sum();  list.Average()
来源：http://cg.wgjwhj.cn

[D17] 最大值与最小值
来源：http://mt.asd995.cn

Py:   max(arr);  min(arr)
来源：http://as.colortex.cn


<!-- 参考信息 -->