代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://tp.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ex.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ux.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://bj.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://zc.jctech888.com.cn

[C03] 可变参数
来源：http://qv.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://ep.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vb.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kx.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mv.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yi.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rs.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fg.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ot.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://mw.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tk.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sw.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kc.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ka.wgjwhj.cn

Java: // 无：用 Builder 模式或 record
来源：http://dy.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://qn.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://fa.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://ny.bjjhwx.cn

[C05] 返回多个值
来源：http://uj.bjjhwx.cn

Py:   return a, b
来源：http://qr.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://an.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vv.szxytkj.cn

TS:   return { a, b };
来源：http://fl.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qg.521024.cn

Go:   return a, b
来源：http://ry.hnjuh.cn

Ruby: return a, b
来源：http://os.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://ed.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://qc.hahajie.cn

Py:   square = lambda x: x * x
来源：http://gr.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hc.panjiajie.cn

JS:   const square = x => x * x;
来源：http://io.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://la.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yj.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zg.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://kc.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bx.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://ky.yuexingan06.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ft.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lm.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dj.lnxyls.cn

TS:   arr.map(String)
来源：http://fb.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fu.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ba.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://cs.lnxyls.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://en.asd995.cn

[C08] 闭包
来源：http://gi.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gl.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eq.gzmigu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ck.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://il.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ji.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zi.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wk.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ab.gzmigu.cn

[C09] 递归
来源：http://nw.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ip.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://we.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nx.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jn.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dg.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ys.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wp.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uh.wgjwhj.cn

[C10] 变量作用域
来源：http://hg.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sf.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nb.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ul.hnjuh.cn

TS:   同 JS
来源：http://qc.szsharing.cn

Java: 方法内为块级作用域
来源：http://vc.shtwfgs.cn

Go:   花括号块级作用域
来源：http://hr.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ec.9csxet.cn

C#:   块级作用域
来源：http://ja.panjiajie.cn

[C11] 模块导入与导出
来源：http://cd.huixiangedu.cn

Py:   from module import func
来源：http://ap.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://al.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pf.huanxung.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://an.wgjwhj.cn

Java: import java.util.List;
来源：http://nh.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aj.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://ja.gzmigu.cn

C#:   using System.Text;
来源：http://dn.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://ug.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://zi.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://ma.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://gm.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://ut.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zb.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://ye.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://wh.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gy.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://qp.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nx.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vt.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ii.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ig.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ai.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://vx.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iu.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ah.muxihuayi.cn

[C14] 泛型函数
来源：http://ew.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pr.asd995.cn

PHP:  // 无泛型
来源：http://ol.jctech888.com.cn

JS:   // 无泛型
来源：http://ut.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xd.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://if.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ua.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://uv.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bn.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://di.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ot.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://ac.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ie.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vm.shxzukj.cn

Java: // 无解构
来源：http://ld.wgjwhj.cn

Go:   // 无解构
来源：http://hq.521024.cn

Ruby: a, b = pair
来源：http://xe.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://yr.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://bv.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eu.newstarts.cn

PHP:  // 无重载
来源：http://hd.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://to.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://ic.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jn.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://jt.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://jt.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hy.panjiajie.cn

================================================================================
来源：http://vj.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://qm.gzmigu.cn

================================================================================
来源：http://ec.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://jj.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pw.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yc.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://os.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vt.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xi.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://ef.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://ls.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ul.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://lj.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eo.shxzskj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rt.9csxet.cn

JS:   arr.push(4);
来源：http://ow.hnjuh.cn

TS:   arr.push(4);
来源：http://kb.colortex.cn

Java: list.add(4);
来源：http://iv.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://bq.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://wl.asd995.cn

C#:   list.Add(4);
来源：http://oa.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://uk.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://hy.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mh.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ad.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://ei.chemitech.net.cn

Java: list.add(0, 0);
来源：http://la.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://at.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qc.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://yp.muxihuayi.cn

[D04] 删除元素
来源：http://yd.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zy.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rh.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oc.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://tw.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yd.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://je.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ud.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bp.muxihuayi.cn

[D05] 访问与修改元素
来源：http://vd.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gc.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sp.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://px.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://mt.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://ar.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://wz.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xs.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cd.nicolike.cn

[D06] 数组长度
来源：http://wq.chemitech.net.cn

Py:   len(arr)
来源：http://zr.haigaiapp.cn

PHP:  count($arr);
来源：http://ha.asd995.cn

JS:   arr.length
来源：http://io.huanxung.cn

TS:   arr.length
来源：http://zw.shxzskj.cn

Java: list.size();
来源：http://kb.huanxung.cn

Go:   len(arr)
来源：http://xo.nicolike.cn

Ruby: arr.length; arr.size
来源：http://uz.yuntaijiaju.cn

C#:   list.Count;
来源：http://jy.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://ja.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cs.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pr.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://ld.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://ov.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://yc.gzmigu.cn

Go:   arr[1:4]
来源：http://qa.hahajie.cn

Ruby: arr[1, 3]
来源：http://dj.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://ro.lnxyls.cn

[D08] 合并两个数组
来源：http://sl.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://go.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://cm.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vu.huixiangedu.cn

TS:   [...a, ...b];
来源：http://vp.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cn.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://co.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://fx.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://kx.9csxet.cn

[D09] 排序（升序）
来源：http://vg.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://cy.nicolike.cn

PHP:  sort($arr);
来源：http://nr.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mc.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uo.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rg.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fx.muxihuayi.cn

Ruby: arr.sort
来源：http://ey.szxytkj.cn

C#:   list.Sort();
来源：http://qz.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fl.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://db.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vo.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gy.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://so.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zx.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://px.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dh.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://so.hnjuh.cn

[D11] 反转数组
来源：http://ve.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://er.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://oq.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ae.huanxung.cn

TS:   [...arr].reverse();
来源：http://ro.shxzukj.cn

Java: Collections.reverse(list);
来源：http://gn.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://rx.nicolike.cn

Ruby: arr.reverse
来源：http://bk.newstarts.cn

C#:   list.Reverse();
来源：http://rz.9csxet.cn

[D12] 查找元素下标
来源：http://xk.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://dc.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bh.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://os.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nw.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sa.asd995.cn

Go:   slices.Index(arr, x)
来源：http://ks.nicolike.cn

Ruby: arr.index(x)
来源：http://xj.521024.cn

C#:   list.IndexOf(x);
来源：http://ry.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://jr.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lj.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zq.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://vl.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://lx.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nd.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://to.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mr.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vy.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://az.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pf.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gn.521024.cn

JS:   arr.map(x => x * 2)
来源：http://pg.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://ww.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zx.panjiajie.cn

Go:   // 手写循环
来源：http://bd.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gj.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vy.huixinmuqiang.cn

[D15] 去重
来源：http://et.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cj.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://nw.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://ru.nicolike.cn

TS:   [...new Set(arr)]
来源：http://nu.huixiangedu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eu.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pr.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://qu.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://rh.colortex.cn

[D16] 求和与平均值
来源：http://il.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uj.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vr.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ch.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bq.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jh.asd995.cn

Go:   // 手写循环累加
来源：http://rv.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bx.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://rq.wgjwhj.cn

[D17] 最大值与最小值
来源：http://xi.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://ym.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://or.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pu.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://gn.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hx.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bq.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://ki.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://ry.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://av.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wj.asd995.cn

PHP:  array_merge(...$nested);
来源：http://od.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wk.muxihuayi.cn

TS:   nested.flat();
来源：http://ka.szsharing.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gg.chemitech.net.cn

Go:   // 手写双层循环
来源：http://ws.bookmarksfly.cn

Ruby: nested.flatten
来源：http://wb.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hw.newstarts.cn

[D19] 按字段分组
来源：http://hp.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gb.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yx.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zu.chemitech.net.cn


<!-- 参考信息 -->