代发 wailian999

[C02] 默认参数
来源：http://kk.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://qv.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sz.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://xv.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://sg.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jb.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gx.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://em.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://rp.hahajie.cn

[C03] 可变参数
来源：http://fy.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://ei.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bv.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bs.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rh.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rw.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jv.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ii.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ar.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://om.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gr.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xd.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ni.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ba.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://ih.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://vd.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://ww.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://vs.521024.cn

[C05] 返回多个值
来源：http://fo.asd995.cn

Py:   return a, b
来源：http://wg.colortex.cn

PHP:  return [$a, $b];
来源：http://to.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://py.chemitech.net.cn

TS:   return { a, b };
来源：http://jc.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wr.jctech888.com.cn

Go:   return a, b
来源：http://my.yuexingan06.cn

Ruby: return a, b
来源：http://ed.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://ol.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://ut.asd995.cn

Py:   square = lambda x: x * x
来源：http://cl.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vp.lnxyls.cn

JS:   const square = x => x * x;
来源：http://om.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://ne.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rr.muxihuayi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gn.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://ss.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uk.521024.cn

[C07] 把函数作为参数传入
来源：http://un.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yq.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pc.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fo.gzmigu.cn

TS:   arr.map(String)
来源：http://bm.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lk.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yn.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://zu.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sl.yuntaijiaju.cn

[C08] 闭包
来源：http://ef.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lg.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lf.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xr.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ng.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ty.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dn.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cf.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xi.szsharing.cn

[C09] 递归
来源：http://aa.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sz.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ar.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sb.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://en.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qo.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zl.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ki.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gx.yuexingan06.cn

[C10] 变量作用域
来源：http://vf.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zs.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bt.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ko.asd995.cn

TS:   同 JS
来源：http://bz.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://rr.hahajie.cn

Go:   花括号块级作用域
来源：http://mp.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fg.haigaiapp.cn

C#:   块级作用域
来源：http://ye.bjjhwx.cn

[C11] 模块导入与导出
来源：http://yn.huanxung.cn

Py:   from module import func
来源：http://dw.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qt.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ch.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sd.shxzskj.cn

Java: import java.util.List;
来源：http://hb.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vq.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://dn.lnxyls.cn

C#:   using System.Text;
来源：http://fl.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://fz.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://ex.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://xx.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://uj.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://cn.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xm.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://sr.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://tm.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zp.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://ma.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mi.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ko.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sf.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wo.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://de.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://yt.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nq.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cp.bookmarksfly.cn

[C14] 泛型函数
来源：http://jh.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hg.521024.cn

PHP:  // 无泛型
来源：http://qa.asd995.cn

JS:   // 无泛型
来源：http://se.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vt.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://we.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jh.muxihuayi.cn

Ruby: # 无泛型
来源：http://ct.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sv.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://od.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sj.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://am.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yw.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sa.asd995.cn

Java: // 无解构
来源：http://el.shtwfgs.cn

Go:   // 无解构
来源：http://xl.gzmigu.cn

Ruby: a, b = pair
来源：http://oa.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://yq.521024.cn

[C16] 函数 / 方法重载
来源：http://wn.shxzukj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jc.bookmarksfly.cn

PHP:  // 无重载
来源：http://uo.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xn.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://je.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wf.521024.cn

Go:   // 无重载：用不同函数名
来源：http://tc.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://fe.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cl.szsharing.cn

================================================================================
来源：http://ri.shtwfgs.cn

D. 数组 / 列表 / 集合
来源：http://ga.bjjhwx.cn

================================================================================
来源：http://nn.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://tw.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ww.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gb.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rh.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kg.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sm.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://ys.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://cz.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jz.shxzukj.cn

[D02] 追加元素到末尾
来源：http://xc.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iz.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ug.nicolike.cn

JS:   arr.push(4);
来源：http://cg.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://dh.huixiangedu.cn

Java: list.add(4);
来源：http://ap.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://pm.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://ua.9csxet.cn

C#:   list.Add(4);
来源：http://zp.szsharing.cn

[D03] 在指定位置插入元素
来源：http://dq.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://wd.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cj.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tf.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ev.chemitech.net.cn

Java: list.add(0, 0);
来源：http://mn.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ov.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://es.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://cq.nszjky.cn

[D04] 删除元素
来源：http://jf.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jh.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zj.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zs.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://am.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oa.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hx.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mc.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xq.szxytkj.cn

[D05] 访问与修改元素
来源：http://tr.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cm.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qi.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sm.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://om.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://we.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ft.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ot.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oo.wgjwhj.cn

[D06] 数组长度
来源：http://jr.szsharing.cn

Py:   len(arr)
来源：http://ts.hahajie.cn

PHP:  count($arr);
来源：http://ky.bookmarksfly.cn

JS:   arr.length
来源：http://ol.newstarts.cn

TS:   arr.length
来源：http://xt.szsharing.cn

Java: list.size();
来源：http://vd.shtwfgs.cn

Go:   len(arr)
来源：http://pn.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://gt.nicolike.cn

C#:   list.Count;
来源：http://aj.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://mh.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eo.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pf.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://ur.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://kb.hahajie.cn

Java: list.subList(1, 4);
来源：http://wb.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://rh.hahajie.cn

Ruby: arr[1, 3]
来源：http://cf.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://cp.chemitech.net.cn

[D08] 合并两个数组
来源：http://hn.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://si.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://vu.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zg.nszjky.cn

TS:   [...a, ...b];
来源：http://kz.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fa.haigaiapp.cn

Go:   append(a, b...)
来源：http://wt.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://vi.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://as.chemitech.net.cn

[D09] 排序（升序）
来源：http://ka.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://vm.asd995.cn

PHP:  sort($arr);
来源：http://jq.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ng.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xr.colortex.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nk.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cg.asd995.cn

Ruby: arr.sort
来源：http://nw.yuntaijiaju.cn

C#:   list.Sort();
来源：http://ot.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://de.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wa.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://an.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fj.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jc.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jl.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qz.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jn.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://id.asd995.cn

[D11] 反转数组
来源：http://zq.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dz.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://zg.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wc.newstarts.cn

TS:   [...arr].reverse();
来源：http://rh.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://mf.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://kc.newstarts.cn

Ruby: arr.reverse
来源：http://jn.bookmarksfly.cn

C#:   list.Reverse();
来源：http://zo.hnjuh.cn

[D12] 查找元素下标
来源：http://mo.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://ek.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tw.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mn.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vg.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xs.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://fz.nicolike.cn

Ruby: arr.index(x)
来源：http://qa.nicolike.cn

C#:   list.IndexOf(x);
来源：http://xd.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://ec.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cg.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wi.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://oh.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://js.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://da.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://er.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hb.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vn.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://yr.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lk.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qd.521024.cn

JS:   arr.map(x => x * 2)
来源：http://ee.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://kx.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hg.hnjuh.cn

Go:   // 手写循环
来源：http://wx.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jp.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ss.521024.cn

[D15] 去重
来源：http://lu.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ke.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://nm.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://cn.hahajie.cn

TS:   [...new Set(arr)]
来源：http://ne.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gb.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://iz.521024.cn

Ruby: arr.uniq
来源：http://hx.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://af.chemitech.net.cn

[D16] 求和与平均值
来源：http://dw.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xz.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ud.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ea.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ga.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://go.colortex.cn

Go:   // 手写循环累加
来源：http://xi.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dl.jctech888.com.cn

C#:   list.Sum();  list.Average()
来源：http://pa.szsharing.cn

[D17] 最大值与最小值
来源：http://df.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://sn.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://me.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ve.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://ao.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://in.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ny.nicolike.cn

Ruby: arr.max;  arr.min
来源：http://nw.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://yu.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://ao.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ft.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://hu.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xm.nszjky.cn

TS:   nested.flat();
来源：http://ht.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xg.gzmigu.cn

Go:   // 手写双层循环
来源：http://wa.521024.cn

Ruby: nested.flatten
来源：http://lj.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ts.huixiangedu.cn


<!-- 参考信息 -->