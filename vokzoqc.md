代发 wailian999

Java: if (data == null) return;
来源：http://er.chemitech.net.cn

Go:   if data == nil { return }
来源：http://aw.hnjuh.cn

Ruby: return if data.nil?
来源：http://ws.hnjuh.cn

C#:   if (data == null) return;
来源：http://xc.jctech888.com.cn

================================================================================
来源：http://di.huanxung.cn

C. 函数与作用域
来源：http://ww.bookmarksfly.cn

================================================================================
来源：http://zp.shtwfgs.cn

[C01] 定义函数
来源：http://id.521024.cn

Py:   def add(a, b): return a + b
来源：http://zt.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yo.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://xe.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zh.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gj.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wi.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://ln.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://su.chemitech.net.cn

[C02] 默认参数
来源：http://oy.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://tr.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qx.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://vx.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lv.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yj.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pm.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://xz.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://uf.wgjwhj.cn

[C03] 可变参数
来源：http://bz.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://ba.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ob.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://by.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mm.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cg.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dl.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://as.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zb.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://qz.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hh.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ke.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://co.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nh.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://ri.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://zr.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://as.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://rs.shtwfgs.cn

[C05] 返回多个值
来源：http://qu.asd995.cn

Py:   return a, b
来源：http://hv.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://cv.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xe.jianghongdianzi.cn

TS:   return { a, b };
来源：http://qs.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jr.muxihuayi.cn

Go:   return a, b
来源：http://pv.9csxet.cn

Ruby: return a, b
来源：http://np.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://ni.colortex.cn

[C06] 匿名函数 / lambda
来源：http://at.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://ce.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tw.newstarts.cn

JS:   const square = x => x * x;
来源：http://hv.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://mr.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uz.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://of.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://mn.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://js.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://as.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://im.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kx.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bg.szxytkj.cn

TS:   arr.map(String)
来源：http://oi.szsharing.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sq.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wp.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://ol.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ub.hnjuh.cn

[C08] 闭包
来源：http://dg.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vj.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jl.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zs.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rn.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ui.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://is.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mg.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gi.nicolike.cn

[C09] 递归
来源：http://ga.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://li.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ik.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://es.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ni.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xj.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dn.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ov.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xf.nicolike.cn

[C10] 变量作用域
来源：http://jh.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gd.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yx.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ov.lnxyls.cn

TS:   同 JS
来源：http://ac.szsharing.cn

Java: 方法内为块级作用域
来源：http://xc.521024.cn

Go:   花括号块级作用域
来源：http://mg.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fg.gzmigu.cn

C#:   块级作用域
来源：http://ev.shxzskj.cn

[C11] 模块导入与导出
来源：http://pp.hnjuh.cn

Py:   from module import func
来源：http://el.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kk.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://km.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zm.hnjuh.cn

Java: import java.util.List;
来源：http://ja.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kv.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://jn.bjjhwx.cn

C#:   using System.Text;
来源：http://tr.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://dh.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://ec.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://wx.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://rx.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://cs.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mk.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://bc.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://ar.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xm.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://hv.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ni.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mz.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fm.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ra.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ce.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://wm.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iy.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zj.newstarts.cn

[C14] 泛型函数
来源：http://qx.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rs.bookmarksfly.cn

PHP:  // 无泛型
来源：http://xi.colortex.cn

JS:   // 无泛型
来源：http://sn.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zu.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ng.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jj.szxytkj.cn

Ruby: # 无泛型
来源：http://eu.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vj.9csxet.cn

[C15] 解构 / 展开参数
来源：http://xh.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wr.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://jd.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://re.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gq.panjiajie.cn

Java: // 无解构
来源：http://te.huixiangedu.cn

Go:   // 无解构
来源：http://vw.szxytkj.cn

Ruby: a, b = pair
来源：http://rh.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://tg.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://tu.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xp.gzmigu.cn

PHP:  // 无重载
来源：http://ri.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wi.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://nt.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zh.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://tn.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://fg.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jv.colortex.cn

================================================================================
来源：http://me.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://uw.nszjky.cn

================================================================================
来源：http://cw.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://fk.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ij.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eq.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wu.shxzukj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pg.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qm.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://yv.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://wm.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zs.lnxyls.cn

[D02] 追加元素到末尾
来源：http://wn.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ej.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jx.szsharing.cn

JS:   arr.push(4);
来源：http://nt.szsharing.cn

TS:   arr.push(4);
来源：http://qw.wgjwhj.cn

Java: list.add(4);
来源：http://jw.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://gh.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://cb.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://co.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://fg.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://lr.lnxyls.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://po.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://to.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://dg.shxzukj.cn

Java: list.add(0, 0);
来源：http://tt.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qc.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mf.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://iw.gzmigu.cn

[D04] 删除元素
来源：http://vp.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wb.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yh.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ya.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://nw.bookmarksfly.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ij.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dn.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aj.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ez.wgjwhj.cn

[D05] 访问与修改元素
来源：http://ye.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wh.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bg.colortex.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uh.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://us.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://ds.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://ay.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://at.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gt.hnjuh.cn

[D06] 数组长度
来源：http://bb.jianghongdianzi.cn

Py:   len(arr)
来源：http://hu.shxzskj.cn

PHP:  count($arr);
来源：http://cn.gzmigu.cn

JS:   arr.length
来源：http://gp.shxzskj.cn

TS:   arr.length
来源：http://fu.newstarts.cn

Java: list.size();
来源：http://fg.newstarts.cn

Go:   len(arr)
来源：http://iv.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://vo.shtwfgs.cn

C#:   list.Count;
来源：http://ym.nicolike.cn

[D07] 切片 / 取子数组
来源：http://my.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zi.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hi.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://pt.colortex.cn

TS:   arr.slice(1, 4);
来源：http://eb.shxzukj.cn

Java: list.subList(1, 4);
来源：http://ij.szxytkj.cn

Go:   arr[1:4]
来源：http://bu.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://qg.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://oi.szxytkj.cn

[D08] 合并两个数组
来源：http://wt.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://wd.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://ny.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://an.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://jl.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ed.lnxyls.cn

Go:   append(a, b...)
来源：http://ke.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://qo.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://sr.9csxet.cn

[D09] 排序（升序）
来源：http://tt.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://ak.lnxyls.cn

PHP:  sort($arr);
来源：http://fp.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gy.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://aw.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xm.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ek.haigaiapp.cn

Ruby: arr.sort
来源：http://uw.jctech888.com.cn

C#:   list.Sort();
来源：http://oe.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ab.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lk.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mw.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vs.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oi.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qj.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://np.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dn.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xx.haigaiapp.cn

[D11] 反转数组
来源：http://rt.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cf.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://te.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ql.nszjky.cn

TS:   [...arr].reverse();
来源：http://eo.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://pl.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://ip.hahajie.cn

Ruby: arr.reverse
来源：http://ti.szsharing.cn

C#:   list.Reverse();
来源：http://ah.jctech888.com.cn

[D12] 查找元素下标
来源：http://pl.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://mo.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jl.shxzskj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nl.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nf.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dm.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://rj.lnxyls.cn

Ruby: arr.index(x)
来源：http://ya.huanxung.cn

C#:   list.IndexOf(x);
来源：http://zi.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://ff.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://po.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rq.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://xq.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://hq.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kz.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lr.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wy.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yj.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://me.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rz.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jg.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://bk.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://rl.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ol.chemitech.net.cn

Go:   // 手写循环
来源：http://iw.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ga.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://st.yuntaijiaju.cn

[D15] 去重
来源：http://qb.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zw.shxzskj.cn

PHP:  array_unique($arr);
来源：http://yy.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://hv.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://nc.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fu.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lx.bjjhwx.cn

Ruby: arr.uniq
来源：http://ar.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://fb.huixiangedu.cn

[D16] 求和与平均值
来源：http://iu.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lh.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sa.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ep.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jz.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sm.yuexingan06.cn

Go:   // 手写循环累加
来源：http://aq.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ep.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://ac.asd995.cn

[D17] 最大值与最小值
来源：http://fz.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://ty.muxihuayi.cn


<!-- 参考信息 -->