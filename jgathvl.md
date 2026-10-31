代发 wailian999

================================================================================
来源：http://ms.lnxyls.cn

C. 函数与作用域
来源：http://wi.huixiangedu.cn

================================================================================
来源：http://hl.colortex.cn

[C01] 定义函数
来源：http://qf.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://kb.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uc.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://sb.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lx.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ls.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ot.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://lt.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mc.shtwfgs.cn

[C02] 默认参数
来源：http://qn.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://eq.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ap.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://ro.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ot.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qr.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zx.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://yo.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://fz.nicolike.cn

[C03] 可变参数
来源：http://yq.521024.cn

Py:   def total(*args): return sum(args)
来源：http://jh.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ic.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vn.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bl.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rz.szsharing.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zs.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oc.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oq.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://kw.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ik.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xy.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fr.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gw.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://vt.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://fj.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://wo.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://qq.chemitech.net.cn

[C05] 返回多个值
来源：http://bo.lnxyls.cn

Py:   return a, b
来源：http://ql.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://cz.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fe.colortex.cn

TS:   return { a, b };
来源：http://ki.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rm.521024.cn

Go:   return a, b
来源：http://jl.hahajie.cn

Ruby: return a, b
来源：http://xq.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://nl.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://sm.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://jw.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yl.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://kp.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://vz.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vw.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wr.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://ws.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yq.9csxet.cn

[C07] 把函数作为参数传入
来源：http://fb.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pc.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mr.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vr.panjiajie.cn

TS:   arr.map(String)
来源：http://vg.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kr.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zg.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://cp.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fn.shxzskj.cn

[C08] 闭包
来源：http://jm.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zr.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://py.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gi.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ep.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sv.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kf.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://le.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ut.huanxung.cn

[C09] 递归
来源：http://wr.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mo.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ma.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hs.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uf.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fv.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fj.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wo.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wu.jianghongdianzi.cn

[C10] 变量作用域
来源：http://qh.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sd.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ey.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zi.newstarts.cn

TS:   同 JS
来源：http://vv.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://lz.shtwfgs.cn

Go:   花括号块级作用域
来源：http://ft.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eb.szsharing.cn

C#:   块级作用域
来源：http://do.521024.cn

[C11] 模块导入与导出
来源：http://ff.panjiajie.cn

Py:   from module import func
来源：http://nj.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ti.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://va.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ux.szsharing.cn

Java: import java.util.List;
来源：http://dl.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yt.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://in.hnjuh.cn

C#:   using System.Text;
来源：http://ek.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://im.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://oi.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://ao.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://fy.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://iu.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uy.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://ga.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://sl.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hr.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://rd.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gj.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zf.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://az.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xs.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hu.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://eq.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vw.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://je.bjjhwx.cn

[C14] 泛型函数
来源：http://hw.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nf.wgjwhj.cn

PHP:  // 无泛型
来源：http://ku.521024.cn

JS:   // 无泛型
来源：http://bq.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cy.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gn.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nw.9csxet.cn

Ruby: # 无泛型
来源：http://pe.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wx.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://nx.yuntaijiaju.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://of.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://mt.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vs.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vh.shxzskj.cn

Java: // 无解构
来源：http://ri.jctech888.com.cn

Go:   // 无解构
来源：http://jo.wgjwhj.cn

Ruby: a, b = pair
来源：http://yz.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://su.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://fi.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hs.panjiajie.cn

PHP:  // 无重载
来源：http://xl.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wa.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://ub.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://py.muxihuayi.cn

Go:   // 无重载：用不同函数名
来源：http://dr.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://fu.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mb.haigaiapp.cn

================================================================================
来源：http://hs.asd995.cn

D. 数组 / 列表 / 集合
来源：http://fo.jianghongdianzi.cn

================================================================================
来源：http://fq.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://cn.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vk.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ik.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xu.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hs.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sq.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://by.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://qr.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ok.shxzskj.cn

[D02] 追加元素到末尾
来源：http://in.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ov.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uu.huanxung.cn

JS:   arr.push(4);
来源：http://uq.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://vz.muxihuayi.cn

Java: list.add(4);
来源：http://jn.521024.cn

Go:   arr = append(arr, 4)
来源：http://rn.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://lc.haigaiapp.cn

C#:   list.Add(4);
来源：http://xm.asd995.cn

[D03] 在指定位置插入元素
来源：http://yw.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://rd.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ic.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ch.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://mc.yuexingan06.cn

Java: list.add(0, 0);
来源：http://qy.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://op.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ju.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://yt.haigaiapp.cn

[D04] 删除元素
来源：http://ol.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qa.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ep.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aa.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://ai.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lr.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mi.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jl.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tf.shxzskj.cn

[D05] 访问与修改元素
来源：http://cw.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bv.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fo.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ks.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://gk.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://jt.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://fe.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nw.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ik.huanxung.cn

[D06] 数组长度
来源：http://mi.bjjhwx.cn

Py:   len(arr)
来源：http://vx.asd995.cn

PHP:  count($arr);
来源：http://dv.szsharing.cn

JS:   arr.length
来源：http://uk.9csxet.cn

TS:   arr.length
来源：http://tx.szxytkj.cn

Java: list.size();
来源：http://fn.huixiangedu.cn

Go:   len(arr)
来源：http://fe.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://sz.lnxyls.cn

C#:   list.Count;
来源：http://ac.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://wa.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vl.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gq.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://xa.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://jh.lnxyls.cn

Java: list.subList(1, 4);
来源：http://do.bookmarksfly.cn

Go:   arr[1:4]
来源：http://ea.nicolike.cn

Ruby: arr[1, 3]
来源：http://re.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://cz.nszjky.cn

[D08] 合并两个数组
来源：http://uf.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://qo.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://pm.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pc.yuexingan06.cn

TS:   [...a, ...b];
来源：http://gb.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wu.hahajie.cn

Go:   append(a, b...)
来源：http://ao.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://xy.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://cx.asd995.cn

[D09] 排序（升序）
来源：http://py.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://by.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://pm.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xw.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wu.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ir.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eh.shtwfgs.cn

Ruby: arr.sort
来源：http://qj.bjjhwx.cn

C#:   list.Sort();
来源：http://rp.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tu.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hi.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tz.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rv.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rj.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ii.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ko.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yn.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ws.nszjky.cn

[D11] 反转数组
来源：http://il.hahajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hl.nicolike.cn

PHP:  array_reverse($arr);
来源：http://qy.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pl.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://ds.hnjuh.cn

Java: Collections.reverse(list);
来源：http://sr.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://xo.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://tw.shxzukj.cn

C#:   list.Reverse();
来源：http://xo.gzmigu.cn

[D12] 查找元素下标
来源：http://em.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://bc.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ph.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ih.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ib.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bt.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://of.newstarts.cn

Ruby: arr.index(x)
来源：http://od.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://bp.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://lt.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rf.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://or.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://uh.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://pj.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nl.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ms.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wi.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dz.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://se.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ej.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vo.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://ag.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://xp.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mu.bookmarksfly.cn

Go:   // 手写循环
来源：http://da.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://go.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yo.newstarts.cn

[D15] 去重
来源：http://yg.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cv.hnjuh.cn

PHP:  array_unique($arr);
来源：http://he.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://ne.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://au.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lj.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hj.huixiangedu.cn

Ruby: arr.uniq
来源：http://ns.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://cs.hnjuh.cn

[D16] 求和与平均值
来源：http://vz.muxihuayi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ci.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sb.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hb.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jw.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zo.newstarts.cn

Go:   // 手写循环累加
来源：http://ol.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rr.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://ic.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://ep.asd995.cn

Py:   max(arr);  min(arr)
来源：http://bc.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://zv.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qo.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://fb.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jq.chemitech.net.cn


<!-- 参考信息 -->