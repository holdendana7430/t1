代发 wailian999

Go:   a && b || !c
来源：http://lg.muxihuayi.cn

Ruby: a && b || !c
来源：http://dq.jianghongdianzi.cn

C#:   a && b || !c
来源：http://am.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ua.szxytkj.cn

Py:   if not data: return
来源：http://gy.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://vf.nszjky.cn

JS:   if (!data) return;
来源：http://mz.shtwfgs.cn

TS:   if (!data) return;
来源：http://wb.9csxet.cn

Java: if (data == null) return;
来源：http://pr.gzmigu.cn

Go:   if data == nil { return }
来源：http://gn.shxzukj.cn

Ruby: return if data.nil?
来源：http://gn.colortex.cn

C#:   if (data == null) return;
来源：http://cb.yuntaijiaju.cn

================================================================================
来源：http://jc.521024.cn

C. 函数与作用域
来源：http://ts.bookmarksfly.cn

================================================================================
来源：http://dd.jianghongdianzi.cn

[C01] 定义函数
来源：http://tf.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://kp.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://re.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://ar.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ah.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vp.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sc.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://hf.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zz.panjiajie.cn

[C02] 默认参数
来源：http://gi.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://wz.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ut.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://jk.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hp.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ri.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ew.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://jp.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://ff.gzmigu.cn

[C03] 可变参数
来源：http://jl.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://lg.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gz.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cs.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ba.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rc.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rm.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ag.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qp.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://gx.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fb.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jq.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ye.gzmigu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pt.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://ri.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://ib.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://ee.521024.cn

C#:   f(a: 1, b: 2)
来源：http://yn.yuntaijiaju.cn

[C05] 返回多个值
来源：http://sg.newstarts.cn

Py:   return a, b
来源：http://qv.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://yn.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yx.chemitech.net.cn

TS:   return { a, b };
来源：http://hh.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://am.9csxet.cn

Go:   return a, b
来源：http://ya.haigaiapp.cn

Ruby: return a, b
来源：http://yt.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://jg.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://ho.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://sz.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uv.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://vs.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://se.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mf.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mz.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://qb.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dn.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://pc.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ar.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rg.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gl.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://gs.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bf.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vj.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://em.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://an.nszjky.cn

[C08] 闭包
来源：http://nc.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ca.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yk.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ij.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ls.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gj.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mx.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wh.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mo.yuntaijiaju.cn

[C09] 递归
来源：http://wv.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vh.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ly.colortex.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vk.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kh.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nj.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zg.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://de.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tm.shxzukj.cn

[C10] 变量作用域
来源：http://bz.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ia.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://id.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wx.colortex.cn

TS:   同 JS
来源：http://ls.9csxet.cn

Java: 方法内为块级作用域
来源：http://io.shtwfgs.cn

Go:   花括号块级作用域
来源：http://zc.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wt.colortex.cn

C#:   块级作用域
来源：http://xb.lnxyls.cn

[C11] 模块导入与导出
来源：http://jn.yuntaijiaju.cn

Py:   from module import func
来源：http://on.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ls.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ds.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ce.newstarts.cn

Java: import java.util.List;
来源：http://pu.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cc.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://bz.huixinmuqiang.cn

C#:   using System.Text;
来源：http://yi.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://hb.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://nk.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://nk.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://mr.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://ft.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ft.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://ga.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://wk.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://au.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://ue.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qr.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://at.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zh.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://di.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vj.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://kx.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fl.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://li.521024.cn

[C14] 泛型函数
来源：http://fa.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uy.haigaiapp.cn

PHP:  // 无泛型
来源：http://gn.bjjhwx.cn

JS:   // 无泛型
来源：http://at.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yu.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eh.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nf.hnjuh.cn

Ruby: # 无泛型
来源：http://zd.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vh.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://bn.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vs.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://pj.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zq.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://up.shtwfgs.cn

Java: // 无解构
来源：http://wv.hahajie.cn

Go:   // 无解构
来源：http://cu.asd995.cn

Ruby: a, b = pair
来源：http://ux.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://dz.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://rc.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qi.yuntaijiaju.cn

PHP:  // 无重载
来源：http://cj.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://up.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://ex.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://np.nicolike.cn

Go:   // 无重载：用不同函数名
来源：http://rx.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://bp.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yr.szxytkj.cn

================================================================================
来源：http://ti.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://dg.asd995.cn

================================================================================
来源：http://ws.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://sp.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kf.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nk.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yp.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ql.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nl.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://ye.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://vg.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wq.shxzskj.cn

[D02] 追加元素到末尾
来源：http://ht.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gq.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://re.huixiangedu.cn

JS:   arr.push(4);
来源：http://bl.colortex.cn

TS:   arr.push(4);
来源：http://rk.nszjky.cn

Java: list.add(4);
来源：http://nv.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://vy.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://xb.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://va.9csxet.cn

[D03] 在指定位置插入元素
来源：http://mp.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://od.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tm.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jr.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://mq.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://nd.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vn.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jc.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://mo.bjjhwx.cn

[D04] 删除元素
来源：http://sz.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ci.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://da.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lq.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://yr.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nq.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aj.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://it.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sw.chemitech.net.cn

[D05] 访问与修改元素
来源：http://rw.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://am.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kg.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ph.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://nh.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://ek.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://jt.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tv.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://js.muxihuayi.cn

[D06] 数组长度
来源：http://jb.wgjwhj.cn

Py:   len(arr)
来源：http://kt.colortex.cn

PHP:  count($arr);
来源：http://lq.hahajie.cn

JS:   arr.length
来源：http://tq.lnxyls.cn

TS:   arr.length
来源：http://qh.huixiangedu.cn

Java: list.size();
来源：http://xp.huixinmuqiang.cn

Go:   len(arr)
来源：http://lp.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://ih.9csxet.cn

C#:   list.Count;
来源：http://rt.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://zc.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ln.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kb.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://gn.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://jb.hahajie.cn

Java: list.subList(1, 4);
来源：http://zj.huixiangedu.cn

Go:   arr[1:4]
来源：http://hl.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://xl.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://xi.wgjwhj.cn

[D08] 合并两个数组
来源：http://oi.521024.cn

Py:   a + b;  a.extend(b)
来源：http://ll.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://qd.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pv.hahajie.cn

TS:   [...a, ...b];
来源：http://dk.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sv.lnxyls.cn

Go:   append(a, b...)
来源：http://sd.bookmarksfly.cn

Ruby: a + b;  a.concat(b)
来源：http://pi.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://pr.yuexingan06.cn

[D09] 排序（升序）
来源：http://ic.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://cs.haigaiapp.cn

PHP:  sort($arr);
来源：http://ei.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xk.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tc.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tl.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pl.shtwfgs.cn

Ruby: arr.sort
来源：http://nz.panjiajie.cn

C#:   list.Sort();
来源：http://ia.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dm.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gr.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wo.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uj.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lt.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dq.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hu.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xv.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qe.lnxyls.cn

[D11] 反转数组
来源：http://xm.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gg.9csxet.cn

PHP:  array_reverse($arr);
来源：http://tf.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ia.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://hn.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://nj.asd995.cn

Go:   slices.Reverse(arr)
来源：http://rx.bjjhwx.cn

Ruby: arr.reverse
来源：http://ae.asd995.cn

C#:   list.Reverse();
来源：http://ep.jctech888.com.cn

[D12] 查找元素下标
来源：http://zr.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://ye.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xb.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qe.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fn.nszjky.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://te.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://gb.huixiangedu.cn

Ruby: arr.index(x)
来源：http://yw.521024.cn

C#:   list.IndexOf(x);
来源：http://fl.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://jl.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ok.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://up.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://kd.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://ki.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://su.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ee.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://aa.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pp.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://gr.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lm.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yj.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://vj.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://ds.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ld.muxihuayi.cn

Go:   // 手写循环
来源：http://ol.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yf.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wt.szxytkj.cn

[D15] 去重
来源：http://oo.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yg.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://vh.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://om.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://lt.huixiangedu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gm.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bl.yuexingan06.cn

Ruby: arr.uniq
来源：http://oe.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://yt.wgjwhj.cn

[D16] 求和与平均值
来源：http://tf.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jx.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zr.wgjwhj.cn


<!-- 参考信息 -->