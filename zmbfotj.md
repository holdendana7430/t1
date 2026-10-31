代发 wailian999

PHP:  $a && $b || !$c
来源：http://pc.colortex.cn

JS:   a && b || !c
来源：http://aw.wgjwhj.cn

TS:   a && b || !c
来源：http://zq.yuntaijiaju.cn

Java: a && b || !c
来源：http://xi.shxzskj.cn

Go:   a && b || !c
来源：http://kq.shxzukj.cn

Ruby: a && b || !c
来源：http://gk.bookmarksfly.cn

C#:   a && b || !c
来源：http://cq.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zg.9csxet.cn

Py:   if not data: return
来源：http://ms.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://lb.colortex.cn

JS:   if (!data) return;
来源：http://ph.nszjky.cn

TS:   if (!data) return;
来源：http://ir.colortex.cn

Java: if (data == null) return;
来源：http://av.colortex.cn

Go:   if data == nil { return }
来源：http://kc.asd995.cn

Ruby: return if data.nil?
来源：http://sb.jctech888.com.cn

C#:   if (data == null) return;
来源：http://br.shxzukj.cn

================================================================================
来源：http://hq.jianghongdianzi.cn

C. 函数与作用域
来源：http://pv.chemitech.net.cn

================================================================================
来源：http://dt.szxytkj.cn

[C01] 定义函数
来源：http://vg.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://ag.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cz.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://fu.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://np.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dl.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ak.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://cs.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zk.yuntaijiaju.cn

[C02] 默认参数
来源：http://aa.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://ne.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gk.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://vr.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qj.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zc.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wh.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://dz.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://ya.bjjhwx.cn

[C03] 可变参数
来源：http://jp.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://eo.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nu.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mq.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wk.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vd.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yo.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xa.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fd.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://cc.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jv.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wf.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uo.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://za.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://up.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://kn.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://la.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://by.panjiajie.cn

[C05] 返回多个值
来源：http://vd.nicolike.cn

Py:   return a, b
来源：http://tg.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://nh.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wi.muxihuayi.cn

TS:   return { a, b };
来源：http://fb.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ml.521024.cn

Go:   return a, b
来源：http://fp.panjiajie.cn

Ruby: return a, b
来源：http://dl.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://nx.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://pq.newstarts.cn

Py:   square = lambda x: x * x
来源：http://px.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xl.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://sl.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://gb.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bl.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ja.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://mv.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hf.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://fk.bookmarksfly.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://co.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tp.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wq.haigaiapp.cn

TS:   arr.map(String)
来源：http://wt.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fl.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gt.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://ai.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oe.bjjhwx.cn

[C08] 闭包
来源：http://sr.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jd.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sa.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lr.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rh.colortex.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jo.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wi.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rh.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://je.gzmigu.cn

[C09] 递归
来源：http://jd.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://na.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gx.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ja.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://op.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://et.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eh.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pe.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ol.jianghongdianzi.cn

[C10] 变量作用域
来源：http://zw.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ms.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ud.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wj.lnxyls.cn

TS:   同 JS
来源：http://za.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://pk.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://mw.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hj.jctech888.com.cn

C#:   块级作用域
来源：http://ld.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://mm.szsharing.cn

Py:   from module import func
来源：http://yz.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xu.panjiajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qi.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bs.colortex.cn

Java: import java.util.List;
来源：http://iw.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aw.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://gg.521024.cn

C#:   using System.Text;
来源：http://hl.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://dq.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://kf.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://ui.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://ya.huixinmuqiang.cn

TS:   (() => { console.log("run"); })();
来源：http://us.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qu.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://hl.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://nu.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dq.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://ji.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lb.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bd.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cv.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oh.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vi.nszjky.cn

Go:   func add(a, b int) int
来源：http://nl.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mr.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ey.muxihuayi.cn

[C14] 泛型函数
来源：http://yc.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uy.shxzskj.cn

PHP:  // 无泛型
来源：http://df.jctech888.com.cn

JS:   // 无泛型
来源：http://sw.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://da.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://am.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mb.9csxet.cn

Ruby: # 无泛型
来源：http://ad.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://af.colortex.cn

[C15] 解构 / 展开参数
来源：http://rm.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gr.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://lc.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ik.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fp.nszjky.cn

Java: // 无解构
来源：http://rv.chemitech.net.cn

Go:   // 无解构
来源：http://ox.hnjuh.cn

Ruby: a, b = pair
来源：http://rq.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://eb.szsharing.cn

[C16] 函数 / 方法重载
来源：http://vs.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ll.shxzukj.cn

PHP:  // 无重载
来源：http://km.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yf.shtwfgs.cn

TS:   // 用联合类型或重载签名声明
来源：http://fb.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mf.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://yv.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://mr.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ce.huixinmuqiang.cn

================================================================================
来源：http://uj.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://cs.huanxung.cn

================================================================================
来源：http://fy.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://hy.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jw.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fy.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ew.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ok.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tg.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://ed.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://fz.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pl.gzmigu.cn

[D02] 追加元素到末尾
来源：http://kd.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://go.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ht.jctech888.com.cn

JS:   arr.push(4);
来源：http://ui.nicolike.cn

TS:   arr.push(4);
来源：http://ou.9csxet.cn

Java: list.add(4);
来源：http://hg.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://cf.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://yt.huanxung.cn

C#:   list.Add(4);
来源：http://ny.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://pq.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://wd.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lf.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jj.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://tq.shxzukj.cn

Java: list.add(0, 0);
来源：http://ip.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bc.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qi.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://vb.szsharing.cn

[D04] 删除元素
来源：http://xa.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ae.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gw.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://up.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://aw.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qk.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ie.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jl.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tc.521024.cn

[D05] 访问与修改元素
来源：http://gi.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mq.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wf.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://el.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://jv.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://fb.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://nv.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ds.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gk.chemitech.net.cn

[D06] 数组长度
来源：http://xs.wgjwhj.cn

Py:   len(arr)
来源：http://ev.wgjwhj.cn

PHP:  count($arr);
来源：http://gw.lnxyls.cn

JS:   arr.length
来源：http://mr.jctech888.com.cn

TS:   arr.length
来源：http://ue.jianghongdianzi.cn

Java: list.size();
来源：http://bv.szsharing.cn

Go:   len(arr)
来源：http://pf.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://ts.521024.cn

C#:   list.Count;
来源：http://rx.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://oz.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://se.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jt.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://tg.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://wz.asd995.cn

Java: list.subList(1, 4);
来源：http://va.szsharing.cn

Go:   arr[1:4]
来源：http://ar.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://it.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://by.9csxet.cn

[D08] 合并两个数组
来源：http://ao.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://tn.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://wg.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qe.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://oc.521024.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gt.newstarts.cn

Go:   append(a, b...)
来源：http://xf.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://mx.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://jl.jctech888.com.cn

[D09] 排序（升序）
来源：http://uj.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ne.shxzskj.cn

PHP:  sort($arr);
来源：http://qs.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ah.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lo.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bu.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xy.huixinmuqiang.cn

Ruby: arr.sort
来源：http://wr.huixiangedu.cn

C#:   list.Sort();
来源：http://pq.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mk.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bs.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iw.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bq.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zs.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nc.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fb.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lm.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bx.panjiajie.cn

[D11] 反转数组
来源：http://qx.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bv.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://uo.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ua.9csxet.cn

TS:   [...arr].reverse();
来源：http://ww.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://ro.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://fv.chemitech.net.cn

Ruby: arr.reverse
来源：http://ss.wgjwhj.cn

C#:   list.Reverse();
来源：http://kt.9csxet.cn

[D12] 查找元素下标
来源：http://pa.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://df.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ad.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ht.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://na.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ma.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://no.bjjhwx.cn

Ruby: arr.index(x)
来源：http://zg.szxytkj.cn

C#:   list.IndexOf(x);
来源：http://gs.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://od.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ow.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jd.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://ni.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://ip.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qz.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ph.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vd.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wq.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://rq.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ax.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ai.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://zn.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://zl.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://id.bookmarksfly.cn

Go:   // 手写循环
来源：http://ri.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://aa.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ys.nicolike.cn

[D15] 去重
来源：http://kx.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jq.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://ja.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://tj.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://av.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://he.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sv.szxytkj.cn

Ruby: arr.uniq
来源：http://at.bookmarksfly.cn


<!-- 参考信息 -->