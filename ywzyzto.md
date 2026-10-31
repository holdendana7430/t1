代发 wailian999

Py:   if not data: return
来源：http://dr.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://bt.asd995.cn

JS:   if (!data) return;
来源：http://zh.bookmarksfly.cn

TS:   if (!data) return;
来源：http://eg.bjjhwx.cn

Java: if (data == null) return;
来源：http://an.lnxyls.cn

Go:   if data == nil { return }
来源：http://rm.newstarts.cn

Ruby: return if data.nil?
来源：http://qq.bjjhwx.cn

C#:   if (data == null) return;
来源：http://iz.gzmigu.cn

================================================================================
来源：http://hm.bjjhwx.cn

C. 函数与作用域
来源：http://zz.shxzskj.cn

================================================================================
来源：http://of.huixiangedu.cn

[C01] 定义函数
来源：http://ht.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://te.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cj.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://qu.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ma.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gy.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vh.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://vf.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ds.huixinmuqiang.cn

[C02] 默认参数
来源：http://xa.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://al.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fj.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://tq.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ya.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://iu.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iw.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://zg.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://ii.hnjuh.cn

[C03] 可变参数
来源：http://il.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://pb.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ox.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xq.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vo.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sc.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ms.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vk.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iu.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://dw.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dd.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://su.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mi.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nl.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://qc.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://yh.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://li.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://jx.yuntaijiaju.cn

[C05] 返回多个值
来源：http://am.gzmigu.cn

Py:   return a, b
来源：http://zc.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://vv.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wj.huixiangedu.cn

TS:   return { a, b };
来源：http://of.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xd.panjiajie.cn

Go:   return a, b
来源：http://ij.huanxung.cn

Ruby: return a, b
来源：http://hk.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://pa.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://sy.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://vu.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pg.521024.cn

JS:   const square = x => x * x;
来源：http://ck.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://lp.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gj.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://eb.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://qq.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mk.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://gw.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ts.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ux.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://be.wgjwhj.cn

TS:   arr.map(String)
来源：http://ne.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rw.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xx.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://gt.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pv.bjjhwx.cn

[C08] 闭包
来源：http://di.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hi.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ne.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vy.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vp.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hd.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ua.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fi.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fy.nicolike.cn

[C09] 递归
来源：http://wl.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qg.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mt.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ay.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yn.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mm.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mo.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hy.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ue.yuexingan06.cn

[C10] 变量作用域
来源：http://vx.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vj.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cw.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kb.jianghongdianzi.cn

TS:   同 JS
来源：http://uj.asd995.cn

Java: 方法内为块级作用域
来源：http://aq.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://gs.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tt.jianghongdianzi.cn

C#:   块级作用域
来源：http://cl.huixiangedu.cn

[C11] 模块导入与导出
来源：http://yz.521024.cn

Py:   from module import func
来源：http://yi.yuntaijiaju.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qx.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://df.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://om.9csxet.cn

Java: import java.util.List;
来源：http://bi.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ni.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://ys.gzmigu.cn

C#:   using System.Text;
来源：http://oj.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://el.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://in.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://ml.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://is.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://xi.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nx.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://lc.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://gx.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fi.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://us.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bk.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gd.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uv.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tz.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ac.hahajie.cn

Go:   func add(a, b int) int
来源：http://lf.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ru.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bh.bookmarksfly.cn

[C14] 泛型函数
来源：http://fl.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jm.jctech888.com.cn

PHP:  // 无泛型
来源：http://kf.nszjky.cn

JS:   // 无泛型
来源：http://ay.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fu.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wh.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ar.haigaiapp.cn

Ruby: # 无泛型
来源：http://hh.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uc.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://xl.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nq.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://yj.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lm.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uw.jianghongdianzi.cn

Java: // 无解构
来源：http://qy.gzmigu.cn

Go:   // 无解构
来源：http://bj.bookmarksfly.cn

Ruby: a, b = pair
来源：http://mf.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://be.shxzukj.cn

[C16] 函数 / 方法重载
来源：http://zb.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fq.colortex.cn

PHP:  // 无重载
来源：http://kg.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ae.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://on.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://im.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://ia.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://cm.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ad.shxzskj.cn

================================================================================
来源：http://dh.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://jb.wgjwhj.cn

================================================================================
来源：http://dp.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://at.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ps.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mk.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ls.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rl.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pa.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://rq.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://ls.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jl.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://ve.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ve.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hw.nicolike.cn

JS:   arr.push(4);
来源：http://kc.shxzskj.cn

TS:   arr.push(4);
来源：http://bf.hnjuh.cn

Java: list.add(4);
来源：http://rk.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://id.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://ub.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://tb.huanxung.cn

[D03] 在指定位置插入元素
来源：http://wc.521024.cn

Py:   arr.insert(0, 0)
来源：http://yc.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gg.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qw.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://hk.lnxyls.cn

Java: list.add(0, 0);
来源：http://xh.muxihuayi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://se.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lz.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://xu.szsharing.cn

[D04] 删除元素
来源：http://yg.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dw.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ge.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pn.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://mc.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://el.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ht.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gm.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ek.huanxung.cn

[D05] 访问与修改元素
来源：http://ji.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mk.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xr.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bv.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://xz.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://vy.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://sp.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xf.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wi.hahajie.cn

[D06] 数组长度
来源：http://vb.muxihuayi.cn

Py:   len(arr)
来源：http://bt.haigaiapp.cn

PHP:  count($arr);
来源：http://cc.shxzukj.cn

JS:   arr.length
来源：http://wx.hnjuh.cn

TS:   arr.length
来源：http://yh.colortex.cn

Java: list.size();
来源：http://uk.bjjhwx.cn

Go:   len(arr)
来源：http://hz.hahajie.cn

Ruby: arr.length; arr.size
来源：http://vk.gzmigu.cn

C#:   list.Count;
来源：http://bt.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://jk.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wx.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dr.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://tq.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://xm.shxzukj.cn

Java: list.subList(1, 4);
来源：http://qn.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://pj.shxzukj.cn

Ruby: arr[1, 3]
来源：http://et.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://vm.colortex.cn

[D08] 合并两个数组
来源：http://yz.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://lr.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://wy.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vi.colortex.cn

TS:   [...a, ...b];
来源：http://th.521024.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ug.asd995.cn

Go:   append(a, b...)
来源：http://zi.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://uz.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://uv.huanxung.cn

[D09] 排序（升序）
来源：http://jk.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://rh.bookmarksfly.cn

PHP:  sort($arr);
来源：http://zg.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ia.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yq.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sw.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cq.szxytkj.cn

Ruby: arr.sort
来源：http://vg.huanxung.cn

C#:   list.Sort();
来源：http://mv.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bb.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oj.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cw.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aq.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nh.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lt.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ox.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vo.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fm.huixinmuqiang.cn

[D11] 反转数组
来源：http://sh.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gs.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://ae.shtwfgs.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lt.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://rg.lnxyls.cn

Java: Collections.reverse(list);
来源：http://kn.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://jp.bookmarksfly.cn

Ruby: arr.reverse
来源：http://ys.szsharing.cn

C#:   list.Reverse();
来源：http://kz.colortex.cn

[D12] 查找元素下标
来源：http://fo.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://xr.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sh.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ue.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ns.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://du.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://tx.huixiangedu.cn

Ruby: arr.index(x)
来源：http://bg.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://by.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://gg.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://af.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://di.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://ei.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://rs.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zx.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ql.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rn.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://le.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://wj.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lf.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ze.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://xw.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://tw.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jm.jctech888.com.cn

Go:   // 手写循环
来源：http://vo.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qg.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rn.haigaiapp.cn

[D15] 去重
来源：http://fm.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ei.hnjuh.cn

PHP:  array_unique($arr);
来源：http://uw.asd995.cn

JS:   [...new Set(arr)]
来源：http://fe.szsharing.cn

TS:   [...new Set(arr)]
来源：http://oj.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rf.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ba.hnjuh.cn

Ruby: arr.uniq
来源：http://wx.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://pw.shtwfgs.cn

[D16] 求和与平均值
来源：http://di.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eh.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ts.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fz.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tl.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ji.521024.cn

Go:   // 手写循环累加
来源：http://mz.bookmarksfly.cn


<!-- 参考信息 -->