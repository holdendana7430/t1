代发 wailian999

PHP:  $a && $b || !$c
来源：http://vm.nszjky.cn

JS:   a && b || !c
来源：http://kr.huixiangedu.cn

TS:   a && b || !c
来源：http://dl.haigaiapp.cn

Java: a && b || !c
来源：http://ce.huanxung.cn

Go:   a && b || !c
来源：http://rz.shtwfgs.cn

Ruby: a && b || !c
来源：http://rr.shtwfgs.cn

C#:   a && b || !c
来源：http://mc.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pz.bookmarksfly.cn

Py:   if not data: return
来源：http://hy.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://lz.nszjky.cn

JS:   if (!data) return;
来源：http://tt.asd995.cn

TS:   if (!data) return;
来源：http://kn.shxzskj.cn

Java: if (data == null) return;
来源：http://ri.newstarts.cn

Go:   if data == nil { return }
来源：http://qm.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://eh.gzmigu.cn

C#:   if (data == null) return;
来源：http://bq.chemitech.net.cn

================================================================================
来源：http://rw.szsharing.cn

C. 函数与作用域
来源：http://cy.shxzukj.cn

================================================================================
来源：http://fd.shtwfgs.cn

[C01] 定义函数
来源：http://zm.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://kr.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rj.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://cj.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ux.bjjhwx.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ab.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yq.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://kt.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bl.hnjuh.cn

[C02] 默认参数
来源：http://dv.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://xp.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kq.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://xg.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rt.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://un.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://du.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://kh.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://pj.lnxyls.cn

[C03] 可变参数
来源：http://wi.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://ud.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xl.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fw.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cc.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gp.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qe.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rv.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nx.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://vg.jctech888.com.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ke.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ky.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pk.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cu.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://ba.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://rc.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://yf.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://cl.nicolike.cn

[C05] 返回多个值
来源：http://bc.hahajie.cn

Py:   return a, b
来源：http://pj.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://mp.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yw.yuntaijiaju.cn

TS:   return { a, b };
来源：http://vq.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yb.hahajie.cn

Go:   return a, b
来源：http://ix.newstarts.cn

Ruby: return a, b
来源：http://sg.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://zh.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://te.9csxet.cn

Py:   square = lambda x: x * x
来源：http://ov.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://au.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://ug.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://qj.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pv.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uy.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://bm.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ur.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://dm.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dc.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rv.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ei.chemitech.net.cn

TS:   arr.map(String)
来源：http://tn.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fl.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xg.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://jg.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zh.nicolike.cn

[C08] 闭包
来源：http://hu.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ur.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://li.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cq.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cj.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zs.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://li.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ul.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fn.shxzskj.cn

[C09] 递归
来源：http://vy.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ih.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nk.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pj.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tv.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vn.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dq.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wi.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gj.huanxung.cn

[C10] 变量作用域
来源：http://vr.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hu.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://um.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hj.9csxet.cn

TS:   同 JS
来源：http://un.gzmigu.cn

Java: 方法内为块级作用域
来源：http://et.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://qw.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zm.szsharing.cn

C#:   块级作用域
来源：http://dj.szxytkj.cn

[C11] 模块导入与导出
来源：http://fz.huanxung.cn

Py:   from module import func
来源：http://ps.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vg.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uv.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dg.521024.cn

Java: import java.util.List;
来源：http://qp.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lp.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://vs.gzmigu.cn

C#:   using System.Text;
来源：http://dr.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://oq.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://sk.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://hn.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://cd.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://xg.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ma.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://fk.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://vd.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nu.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://aq.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pj.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gm.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tm.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vo.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sm.szsharing.cn

Go:   func add(a, b int) int
来源：http://ow.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://er.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ty.haigaiapp.cn

[C14] 泛型函数
来源：http://ch.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xn.szsharing.cn

PHP:  // 无泛型
来源：http://yd.jianghongdianzi.cn

JS:   // 无泛型
来源：http://wv.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uj.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ya.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://id.panjiajie.cn

Ruby: # 无泛型
来源：http://zd.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vo.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://no.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dr.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://zo.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xc.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rc.bjjhwx.cn

Java: // 无解构
来源：http://yo.bjjhwx.cn

Go:   // 无解构
来源：http://ak.521024.cn

Ruby: a, b = pair
来源：http://sb.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://es.hahajie.cn

[C16] 函数 / 方法重载
来源：http://gp.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sp.jctech888.com.cn

PHP:  // 无重载
来源：http://qc.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ss.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://jf.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://so.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://ma.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://ol.yuexingan06.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sz.nszjky.cn

================================================================================
来源：http://at.521024.cn

D. 数组 / 列表 / 集合
来源：http://xo.szxytkj.cn

================================================================================
来源：http://im.huanxung.cn

[D01] 创建数组 / 列表
来源：http://zb.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lz.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pj.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qh.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vj.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bu.shtwfgs.cn

Go:   arr := []int{1, 2, 3}
来源：http://sa.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://mp.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ww.lnxyls.cn

[D02] 追加元素到末尾
来源：http://zv.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://du.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fq.jctech888.com.cn

JS:   arr.push(4);
来源：http://ea.shxzukj.cn

TS:   arr.push(4);
来源：http://md.gzmigu.cn

Java: list.add(4);
来源：http://jd.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://kc.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://uk.lnxyls.cn

C#:   list.Add(4);
来源：http://bf.hahajie.cn

[D03] 在指定位置插入元素
来源：http://io.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://pw.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ys.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vg.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://wv.colortex.cn

Java: list.add(0, 0);
来源：http://cv.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mw.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ge.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://kb.chemitech.net.cn

[D04] 删除元素
来源：http://wk.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zu.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ad.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vg.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://ps.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://in.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pg.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zx.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qe.hahajie.cn

[D05] 访问与修改元素
来源：http://lk.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qq.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uk.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cs.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://qd.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://bc.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://we.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://da.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mu.colortex.cn

[D06] 数组长度
来源：http://kr.shxzskj.cn

Py:   len(arr)
来源：http://fs.newstarts.cn

PHP:  count($arr);
来源：http://hw.chemitech.net.cn

JS:   arr.length
来源：http://kp.shxzukj.cn

TS:   arr.length
来源：http://ax.jctech888.com.cn

Java: list.size();
来源：http://zv.hnjuh.cn

Go:   len(arr)
来源：http://ua.9csxet.cn

Ruby: arr.length; arr.size
来源：http://sw.nicolike.cn

C#:   list.Count;
来源：http://of.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://fk.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eo.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fe.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://rp.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://fa.9csxet.cn

Java: list.subList(1, 4);
来源：http://ey.9csxet.cn

Go:   arr[1:4]
来源：http://mo.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://gc.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://wb.newstarts.cn

[D08] 合并两个数组
来源：http://ld.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://ig.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://ln.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pq.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://dn.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gc.haigaiapp.cn

Go:   append(a, b...)
来源：http://su.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://cz.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://lw.shtwfgs.cn

[D09] 排序（升序）
来源：http://gq.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://df.yuexingan06.cn

PHP:  sort($arr);
来源：http://yp.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xf.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oa.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ti.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tp.bjjhwx.cn

Ruby: arr.sort
来源：http://hb.szsharing.cn

C#:   list.Sort();
来源：http://tl.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://eo.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ev.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ws.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zh.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vc.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ix.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kq.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bb.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://my.chemitech.net.cn

[D11] 反转数组
来源：http://hl.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ao.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://dn.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://os.huanxung.cn

TS:   [...arr].reverse();
来源：http://so.newstarts.cn

Java: Collections.reverse(list);
来源：http://uf.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://sz.huixiangedu.cn

Ruby: arr.reverse
来源：http://xq.shxzukj.cn

C#:   list.Reverse();
来源：http://gl.9csxet.cn

[D12] 查找元素下标
来源：http://ih.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://gu.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xg.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qv.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wq.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mf.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://np.nszjky.cn

Ruby: arr.index(x)
来源：http://dl.nszjky.cn

C#:   list.IndexOf(x);
来源：http://vu.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://lo.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tc.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://aq.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://yz.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://oo.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cz.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oe.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dt.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vg.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://wq.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fh.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ie.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://ie.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://ef.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://je.asd995.cn

Go:   // 手写循环
来源：http://zd.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ht.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sj.chemitech.net.cn

[D15] 去重
来源：http://kp.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fk.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://qk.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://zp.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://bu.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yy.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fv.szxytkj.cn

Ruby: arr.uniq
来源：http://av.bookmarksfly.cn


<!-- 参考信息 -->