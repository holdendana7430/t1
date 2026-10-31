代发 wailian999

Py:   if not data: return
来源：http://sb.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://gr.jctech888.com.cn

JS:   if (!data) return;
来源：http://pz.jctech888.com.cn

TS:   if (!data) return;
来源：http://ol.newstarts.cn

Java: if (data == null) return;
来源：http://va.haigaiapp.cn

Go:   if data == nil { return }
来源：http://jr.shxzskj.cn

Ruby: return if data.nil?
来源：http://eu.jctech888.com.cn

C#:   if (data == null) return;
来源：http://pf.9csxet.cn

================================================================================
来源：http://yi.shxzskj.cn

C. 函数与作用域
来源：http://yl.muxihuayi.cn

================================================================================
来源：http://ju.hahajie.cn

[C01] 定义函数
来源：http://ix.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://tz.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ey.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://ac.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ph.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://en.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mh.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://zx.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dl.yuntaijiaju.cn

[C02] 默认参数
来源：http://hn.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://rt.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tg.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://sm.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kz.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cx.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://up.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://fk.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://wm.jctech888.com.cn

[C03] 可变参数
来源：http://pt.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://dq.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sd.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rf.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wt.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ag.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nr.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://if.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iq.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://td.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sm.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wj.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gq.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://za.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://yt.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://zc.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://bj.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://al.szsharing.cn

[C05] 返回多个值
来源：http://dj.huixiangedu.cn

Py:   return a, b
来源：http://bn.colortex.cn

PHP:  return [$a, $b];
来源：http://by.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pm.wgjwhj.cn

TS:   return { a, b };
来源：http://gb.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://px.huixiangedu.cn

Go:   return a, b
来源：http://ci.bookmarksfly.cn

Ruby: return a, b
来源：http://hw.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://vv.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://wn.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://cg.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bg.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://tt.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://nl.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sz.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hw.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://be.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oh.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://rh.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qv.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mp.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pa.haigaiapp.cn

TS:   arr.map(String)
来源：http://rg.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hn.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pz.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://mq.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gc.gzmigu.cn

[C08] 闭包
来源：http://xb.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bi.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hf.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fe.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ig.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zw.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pl.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tt.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iu.huixinmuqiang.cn

[C09] 递归
来源：http://uh.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jq.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wl.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zo.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jp.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://no.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lw.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aa.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rg.newstarts.cn

[C10] 变量作用域
来源：http://kh.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fc.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hr.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rj.bookmarksfly.cn

TS:   同 JS
来源：http://dl.hnjuh.cn

Java: 方法内为块级作用域
来源：http://wp.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://hc.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uk.bookmarksfly.cn

C#:   块级作用域
来源：http://bp.wgjwhj.cn

[C11] 模块导入与导出
来源：http://xj.9csxet.cn

Py:   from module import func
来源：http://tz.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vk.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hk.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jd.colortex.cn

Java: import java.util.List;
来源：http://rm.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qh.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ke.hahajie.cn

C#:   using System.Text;
来源：http://wo.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://gu.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://tz.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://pp.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://ja.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://gd.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ke.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://ya.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://yp.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://at.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://nf.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tm.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://td.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://an.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ja.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ll.gzmigu.cn

Go:   func add(a, b int) int
来源：http://vo.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pk.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fy.szsharing.cn

[C14] 泛型函数
来源：http://ha.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zg.huanxung.cn

PHP:  // 无泛型
来源：http://rh.haigaiapp.cn

JS:   // 无泛型
来源：http://pw.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ey.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dj.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hr.yuexingan06.cn

Ruby: # 无泛型
来源：http://st.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sr.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://zu.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lk.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://rc.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vg.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ih.huanxung.cn

Java: // 无解构
来源：http://hd.szsharing.cn

Go:   // 无解构
来源：http://ob.panjiajie.cn

Ruby: a, b = pair
来源：http://sc.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://aj.nicolike.cn

[C16] 函数 / 方法重载
来源：http://uy.nszjky.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nu.yuntaijiaju.cn

PHP:  // 无重载
来源：http://hn.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hy.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://fy.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ty.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://iw.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://yi.yuexingan06.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cv.9csxet.cn

================================================================================
来源：http://mp.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://fj.shxzskj.cn

================================================================================
来源：http://xh.hahajie.cn

[D01] 创建数组 / 列表
来源：http://if.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ib.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fj.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tz.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xb.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gi.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ct.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://ae.asd995.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uo.szxytkj.cn

[D02] 追加元素到末尾
来源：http://vw.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kg.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pe.huanxung.cn

JS:   arr.push(4);
来源：http://we.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://hi.bjjhwx.cn

Java: list.add(4);
来源：http://tn.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://kq.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://gm.muxihuayi.cn

C#:   list.Add(4);
来源：http://of.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://ub.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://yd.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vu.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gk.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://cb.panjiajie.cn

Java: list.add(0, 0);
来源：http://uz.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jo.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://np.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://ir.chemitech.net.cn

[D04] 删除元素
来源：http://qr.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ju.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zi.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vw.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://sq.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tc.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ja.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fu.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ww.hahajie.cn

[D05] 访问与修改元素
来源：http://zk.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lt.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ds.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uk.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://mg.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://ka.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://ah.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oh.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pc.chemitech.net.cn

[D06] 数组长度
来源：http://xo.yuntaijiaju.cn

Py:   len(arr)
来源：http://ri.colortex.cn

PHP:  count($arr);
来源：http://jx.hnjuh.cn

JS:   arr.length
来源：http://xv.colortex.cn

TS:   arr.length
来源：http://bf.haigaiapp.cn

Java: list.size();
来源：http://bu.9csxet.cn

Go:   len(arr)
来源：http://nt.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://dz.hnjuh.cn

C#:   list.Count;
来源：http://kn.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://ag.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vs.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://la.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://gd.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://wh.szxytkj.cn

Java: list.subList(1, 4);
来源：http://xw.newstarts.cn

Go:   arr[1:4]
来源：http://ml.panjiajie.cn

Ruby: arr[1, 3]
来源：http://ew.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://lj.9csxet.cn

[D08] 合并两个数组
来源：http://fm.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://lt.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://iu.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mf.shxzskj.cn

TS:   [...a, ...b];
来源：http://gw.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rh.panjiajie.cn

Go:   append(a, b...)
来源：http://el.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://ai.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://nb.haigaiapp.cn

[D09] 排序（升序）
来源：http://ul.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://iz.muxihuayi.cn

PHP:  sort($arr);
来源：http://ia.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lz.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gm.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ux.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dl.huixinmuqiang.cn

Ruby: arr.sort
来源：http://hm.bookmarksfly.cn

C#:   list.Sort();
来源：http://dh.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pq.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sv.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xh.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sb.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xv.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nz.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ve.colortex.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://er.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gu.nicolike.cn

[D11] 反转数组
来源：http://ca.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nw.newstarts.cn

PHP:  array_reverse($arr);
来源：http://vx.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xi.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://sc.szxytkj.cn

Java: Collections.reverse(list);
来源：http://jb.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://ur.9csxet.cn

Ruby: arr.reverse
来源：http://wm.chemitech.net.cn

C#:   list.Reverse();
来源：http://nf.shxzukj.cn

[D12] 查找元素下标
来源：http://bx.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://qi.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wd.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wu.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ga.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://du.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://cl.lnxyls.cn

Ruby: arr.index(x)
来源：http://vx.szxytkj.cn

C#:   list.IndexOf(x);
来源：http://ey.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://vw.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wq.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vs.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://pf.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://pk.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qw.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xw.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://px.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tv.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://yn.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kj.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wy.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://dl.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://md.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kt.shxzukj.cn

Go:   // 手写循环
来源：http://po.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rh.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pd.9csxet.cn

[D15] 去重
来源：http://vd.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wq.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://ct.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://rj.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://st.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kg.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wz.wgjwhj.cn

Ruby: arr.uniq
来源：http://ac.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://xl.huixiangedu.cn

[D16] 求和与平均值
来源：http://qh.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://za.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qr.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hf.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fb.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wg.9csxet.cn

Go:   // 手写循环累加
来源：http://yp.muxihuayi.cn


<!-- 参考信息 -->