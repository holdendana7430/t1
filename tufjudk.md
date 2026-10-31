代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://fa.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dm.9csxet.cn

[B15] 布尔运算与取反
来源：http://zv.hnjuh.cn

Py:   a and b or not c
来源：http://px.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://ir.gzmigu.cn

JS:   a && b || !c
来源：http://yr.bjjhwx.cn

TS:   a && b || !c
来源：http://ft.hahajie.cn

Java: a && b || !c
来源：http://vh.gzmigu.cn

Go:   a && b || !c
来源：http://sq.nicolike.cn

Ruby: a && b || !c
来源：http://tj.chemitech.net.cn

C#:   a && b || !c
来源：http://bc.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://to.hahajie.cn

Py:   if not data: return
来源：http://ik.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://nb.shxzukj.cn

JS:   if (!data) return;
来源：http://bc.bookmarksfly.cn

TS:   if (!data) return;
来源：http://am.bookmarksfly.cn

Java: if (data == null) return;
来源：http://ji.haigaiapp.cn

Go:   if data == nil { return }
来源：http://zh.yuexingan06.cn

Ruby: return if data.nil?
来源：http://hg.chemitech.net.cn

C#:   if (data == null) return;
来源：http://vb.colortex.cn

================================================================================
来源：http://vk.newstarts.cn

C. 函数与作用域
来源：http://xl.huanxung.cn

================================================================================
来源：http://po.nicolike.cn

[C01] 定义函数
来源：http://eh.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://px.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pr.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://dn.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gs.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dg.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mp.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://ta.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zd.jianghongdianzi.cn

[C02] 默认参数
来源：http://kq.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://vp.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jm.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://cv.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dz.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://il.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tp.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://mp.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://uv.shxzskj.cn

[C03] 可变参数
来源：http://wv.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://fp.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wx.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://je.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zy.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uv.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vx.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ah.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://ih.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mz.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://et.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bc.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://od.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://ek.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://wl.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://uv.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://bj.yuntaijiaju.cn

[C05] 返回多个值
来源：http://bf.shxzukj.cn

Py:   return a, b
来源：http://dn.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://ro.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yr.hahajie.cn

TS:   return { a, b };
来源：http://at.huixiangedu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sr.chemitech.net.cn

Go:   return a, b
来源：http://ti.haigaiapp.cn

Ruby: return a, b
来源：http://xr.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://sy.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://hs.hahajie.cn

Py:   square = lambda x: x * x
来源：http://pj.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fx.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://ik.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://ch.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tv.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ro.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://yi.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oi.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://rc.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wj.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://it.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://va.shxzukj.cn

TS:   arr.map(String)
来源：http://fa.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tp.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aw.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://me.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ei.jianghongdianzi.cn

[C08] 闭包
来源：http://cm.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jk.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tb.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aw.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wo.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ca.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aj.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mu.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cx.szsharing.cn

[C09] 递归
来源：http://um.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ck.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xj.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yf.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ur.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://or.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vo.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bj.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zp.jctech888.com.cn

[C10] 变量作用域
来源：http://ig.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oh.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jm.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gz.9csxet.cn

TS:   同 JS
来源：http://pb.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://jp.shxzskj.cn

Go:   花括号块级作用域
来源：http://vg.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pe.chemitech.net.cn

C#:   块级作用域
来源：http://dc.yuexingan06.cn

[C11] 模块导入与导出
来源：http://ym.yuexingan06.cn

Py:   from module import func
来源：http://vk.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wf.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lf.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sp.bjjhwx.cn

Java: import java.util.List;
来源：http://ju.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ho.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://as.hnjuh.cn

C#:   using System.Text;
来源：http://iw.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://pz.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://ot.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://xd.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://kw.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://yw.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wh.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://ao.521024.cn

Ruby: -> { puts "run" }.call
来源：http://lo.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dk.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://kr.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xv.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mg.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gv.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dz.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ev.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://vj.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uw.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xv.yuntaijiaju.cn

[C14] 泛型函数
来源：http://es.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qp.nicolike.cn

PHP:  // 无泛型
来源：http://rj.hahajie.cn

JS:   // 无泛型
来源：http://de.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ia.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://or.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bd.hahajie.cn

Ruby: # 无泛型
来源：http://fd.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hd.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://uy.bjjhwx.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tn.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://nx.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eq.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wa.yuexingan06.cn

Java: // 无解构
来源：http://bb.nicolike.cn

Go:   // 无解构
来源：http://nu.bookmarksfly.cn

Ruby: a, b = pair
来源：http://fj.huanxung.cn

C#:   var (a, b) = pair;
来源：http://dr.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://nr.nszjky.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fs.chemitech.net.cn

PHP:  // 无重载
来源：http://an.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zr.shtwfgs.cn

TS:   // 用联合类型或重载签名声明
来源：http://ak.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wg.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://ga.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://yf.colortex.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sb.hnjuh.cn

================================================================================
来源：http://cl.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://ib.521024.cn

================================================================================
来源：http://ml.nszjky.cn

[D01] 创建数组 / 列表
来源：http://ty.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pa.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://in.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nj.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qr.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://eb.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://vx.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://dh.shxzskj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zc.shxzskj.cn

[D02] 追加元素到末尾
来源：http://iv.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bs.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ej.gzmigu.cn

JS:   arr.push(4);
来源：http://tb.gzmigu.cn

TS:   arr.push(4);
来源：http://ji.chemitech.net.cn

Java: list.add(4);
来源：http://yk.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://ht.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://cq.colortex.cn

C#:   list.Add(4);
来源：http://bk.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://bx.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://uj.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ge.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yk.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://zr.bjjhwx.cn

Java: list.add(0, 0);
来源：http://xq.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ry.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sd.muxihuayi.cn

C#:   list.Insert(0, 0);
来源：http://uu.yuexingan06.cn

[D04] 删除元素
来源：http://bl.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ii.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cw.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hn.hnjuh.cn

TS:   arr.splice(0, 1);
来源：http://zk.shxzskj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jc.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oq.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zr.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zb.haigaiapp.cn

[D05] 访问与修改元素
来源：http://si.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wa.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oc.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qj.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://oq.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://qu.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://as.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ie.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gw.521024.cn

[D06] 数组长度
来源：http://or.shxzskj.cn

Py:   len(arr)
来源：http://zv.wgjwhj.cn

PHP:  count($arr);
来源：http://yj.yuexingan06.cn

JS:   arr.length
来源：http://hu.521024.cn

TS:   arr.length
来源：http://pu.huixinmuqiang.cn

Java: list.size();
来源：http://on.szsharing.cn

Go:   len(arr)
来源：http://vl.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://vd.panjiajie.cn

C#:   list.Count;
来源：http://ec.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://uj.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yx.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ik.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://xc.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://ms.521024.cn

Java: list.subList(1, 4);
来源：http://nw.asd995.cn

Go:   arr[1:4]
来源：http://um.shxzukj.cn

Ruby: arr[1, 3]
来源：http://up.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://yj.huanxung.cn

[D08] 合并两个数组
来源：http://ly.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://ir.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://li.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vk.huanxung.cn

TS:   [...a, ...b];
来源：http://ow.jianghongdianzi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pz.521024.cn

Go:   append(a, b...)
来源：http://jx.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://pm.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://ma.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://jo.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://pz.gzmigu.cn

PHP:  sort($arr);
来源：http://sg.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pc.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://aq.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ba.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hi.gzmigu.cn

Ruby: arr.sort
来源：http://ha.521024.cn

C#:   list.Sort();
来源：http://vw.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ym.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nb.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eb.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ow.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kg.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lw.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ez.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bg.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://of.hnjuh.cn

[D11] 反转数组
来源：http://qx.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gb.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://xc.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fz.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://lg.panjiajie.cn

Java: Collections.reverse(list);
来源：http://ha.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://oe.jctech888.com.cn

Ruby: arr.reverse
来源：http://au.shxzskj.cn

C#:   list.Reverse();
来源：http://fv.hnjuh.cn

[D12] 查找元素下标
来源：http://oj.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://yf.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ev.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cj.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hc.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oe.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://vt.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://ck.521024.cn

C#:   list.IndexOf(x);
来源：http://ll.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://oy.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pj.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bc.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://zl.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://gk.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://up.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rc.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tj.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://la.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://kq.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dq.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jo.521024.cn

JS:   arr.map(x => x * 2)
来源：http://ye.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://ij.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sh.lnxyls.cn

Go:   // 手写循环
来源：http://hw.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bs.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zs.wgjwhj.cn

[D15] 去重
来源：http://gr.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gr.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://yc.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://ju.nicolike.cn


<!-- 参考信息 -->