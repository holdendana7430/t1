代发 wailian999

PHP:  $a && $b || !$c
来源：http://fh.521024.cn

JS:   a && b || !c
来源：http://gb.hahajie.cn

TS:   a && b || !c
来源：http://qd.nicolike.cn

Java: a && b || !c
来源：http://ic.panjiajie.cn

Go:   a && b || !c
来源：http://ve.haigaiapp.cn

Ruby: a && b || !c
来源：http://zm.szxytkj.cn

C#:   a && b || !c
来源：http://ke.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ro.bjjhwx.cn

Py:   if not data: return
来源：http://hq.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://sr.newstarts.cn

JS:   if (!data) return;
来源：http://ws.lnxyls.cn

TS:   if (!data) return;
来源：http://or.nszjky.cn

Java: if (data == null) return;
来源：http://vs.szsharing.cn

Go:   if data == nil { return }
来源：http://nl.9csxet.cn

Ruby: return if data.nil?
来源：http://sp.muxihuayi.cn

C#:   if (data == null) return;
来源：http://ol.szxytkj.cn

================================================================================
来源：http://br.szxytkj.cn

C. 函数与作用域
来源：http://af.panjiajie.cn

================================================================================
来源：http://yh.asd995.cn

[C01] 定义函数
来源：http://nf.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://ni.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zz.huixiangedu.cn

JS:   function add(a, b) { return a + b; }
来源：http://je.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cd.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ww.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pb.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://kc.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yn.yuntaijiaju.cn

[C02] 默认参数
来源：http://th.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://ul.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uy.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://di.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://op.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fi.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wj.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://iq.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://on.muxihuayi.cn

[C03] 可变参数
来源：http://hp.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://mi.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zw.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pc.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kk.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://do.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ns.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cq.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://in.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://wu.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ml.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uj.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gw.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fq.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://tb.521024.cn

Go:   // 无：用配置结构体参数
来源：http://vo.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://lp.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://dk.yuexingan06.cn

[C05] 返回多个值
来源：http://ki.bjjhwx.cn

Py:   return a, b
来源：http://ka.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://jz.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dg.shxzukj.cn

TS:   return { a, b };
来源：http://zv.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vi.colortex.cn

Go:   return a, b
来源：http://or.shxzskj.cn

Ruby: return a, b
来源：http://yp.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://xi.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://bc.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://ok.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gp.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://zi.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://yr.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xw.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qt.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://cp.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://iz.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://om.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wc.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yi.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ll.nicolike.cn

TS:   arr.map(String)
来源：http://vb.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kq.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ah.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://va.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lt.shxzskj.cn

[C08] 闭包
来源：http://ar.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sz.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://no.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rm.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://km.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://co.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hd.huixiangedu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mp.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qn.shxzskj.cn

[C09] 递归
来源：http://hu.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rl.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kb.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bm.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zw.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wz.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ob.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ns.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gw.lnxyls.cn

[C10] 变量作用域
来源：http://tw.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fd.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://th.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bs.nszjky.cn

TS:   同 JS
来源：http://pv.colortex.cn

Java: 方法内为块级作用域
来源：http://vw.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://at.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bz.hahajie.cn

C#:   块级作用域
来源：http://yo.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://nl.panjiajie.cn

Py:   from module import func
来源：http://xg.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vz.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rh.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yn.nicolike.cn

Java: import java.util.List;
来源：http://ro.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wh.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://uq.huanxung.cn

C#:   using System.Text;
来源：http://tk.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://qh.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://vr.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://yb.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://cx.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://nv.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nm.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://yz.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://eg.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mg.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://mx.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hs.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wm.521024.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tc.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zl.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yw.9csxet.cn

Go:   func add(a, b int) int
来源：http://vk.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zk.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xw.chemitech.net.cn

[C14] 泛型函数
来源：http://vv.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pf.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://wz.huixinmuqiang.cn

JS:   // 无泛型
来源：http://cg.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ni.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ug.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nr.yuexingan06.cn

Ruby: # 无泛型
来源：http://bz.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nt.colortex.cn

[C15] 解构 / 展开参数
来源：http://vd.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nv.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://bf.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rf.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dw.asd995.cn

Java: // 无解构
来源：http://gw.bookmarksfly.cn

Go:   // 无解构
来源：http://no.huixiangedu.cn

Ruby: a, b = pair
来源：http://iv.szsharing.cn

C#:   var (a, b) = pair;
来源：http://cd.hahajie.cn

[C16] 函数 / 方法重载
来源：http://go.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zg.huixiangedu.cn

PHP:  // 无重载
来源：http://qy.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bb.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://rb.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://py.huixinmuqiang.cn

Go:   // 无重载：用不同函数名
来源：http://ai.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://hj.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ng.panjiajie.cn

================================================================================
来源：http://jw.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://nv.jianghongdianzi.cn

================================================================================
来源：http://bp.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://ce.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ec.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kh.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bq.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fx.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mb.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ne.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://hb.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gw.szsharing.cn

[D02] 追加元素到末尾
来源：http://gg.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://br.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lt.bookmarksfly.cn

JS:   arr.push(4);
来源：http://pb.colortex.cn

TS:   arr.push(4);
来源：http://ds.chemitech.net.cn

Java: list.add(4);
来源：http://zf.nszjky.cn

Go:   arr = append(arr, 4)
来源：http://sv.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://jl.wgjwhj.cn

C#:   list.Add(4);
来源：http://po.asd995.cn

[D03] 在指定位置插入元素
来源：http://gt.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://wh.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sq.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rs.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://lo.wgjwhj.cn

Java: list.add(0, 0);
来源：http://ud.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zw.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bu.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://ia.newstarts.cn

[D04] 删除元素
来源：http://iv.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dn.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://is.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ui.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://cc.bookmarksfly.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ul.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nf.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sd.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pn.shtwfgs.cn

[D05] 访问与修改元素
来源：http://ea.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://as.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ws.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zr.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://wd.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://ux.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://lt.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rt.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dq.haigaiapp.cn

[D06] 数组长度
来源：http://kj.bjjhwx.cn

Py:   len(arr)
来源：http://ql.szsharing.cn

PHP:  count($arr);
来源：http://zn.huixiangedu.cn

JS:   arr.length
来源：http://kc.yuntaijiaju.cn

TS:   arr.length
来源：http://pe.9csxet.cn

Java: list.size();
来源：http://lv.muxihuayi.cn

Go:   len(arr)
来源：http://pz.colortex.cn

Ruby: arr.length; arr.size
来源：http://vz.shxzukj.cn

C#:   list.Count;
来源：http://tw.colortex.cn

[D07] 切片 / 取子数组
来源：http://mo.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ma.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pt.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://wl.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://ty.nszjky.cn

Java: list.subList(1, 4);
来源：http://xa.gzmigu.cn

Go:   arr[1:4]
来源：http://ti.huanxung.cn

Ruby: arr[1, 3]
来源：http://gy.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://ao.panjiajie.cn

[D08] 合并两个数组
来源：http://qq.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://sb.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://ev.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xz.hnjuh.cn

TS:   [...a, ...b];
来源：http://nu.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ob.9csxet.cn

Go:   append(a, b...)
来源：http://da.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://kb.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://wy.bjjhwx.cn

[D09] 排序（升序）
来源：http://io.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://hr.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://yi.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://we.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zf.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kq.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mq.shxzukj.cn

Ruby: arr.sort
来源：http://sk.9csxet.cn

C#:   list.Sort();
来源：http://lx.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ag.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zl.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xf.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qy.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tm.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://da.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zz.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lg.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mk.shtwfgs.cn

[D11] 反转数组
来源：http://mb.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nh.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://nj.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fp.szsharing.cn

TS:   [...arr].reverse();
来源：http://vv.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://at.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://jd.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://dm.hahajie.cn

C#:   list.Reverse();
来源：http://pb.hnjuh.cn

[D12] 查找元素下标
来源：http://sr.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://sp.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nm.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kw.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ys.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xn.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://or.lnxyls.cn

Ruby: arr.index(x)
来源：http://ys.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://fw.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://mx.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://he.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://du.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://po.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://wu.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iu.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fz.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ec.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qz.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://pm.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pt.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zj.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://om.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://cp.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gc.yuexingan06.cn

Go:   // 手写循环
来源：http://nr.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qd.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ch.lnxyls.cn

[D15] 去重
来源：http://fn.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yj.newstarts.cn

PHP:  array_unique($arr);
来源：http://qn.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://xj.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://sf.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kg.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dw.huixiangedu.cn

Ruby: arr.uniq
来源：http://hi.521024.cn


<!-- 参考信息 -->