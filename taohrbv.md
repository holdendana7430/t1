代发 wailian999

Py:   def add(a, b): return a + b
来源：http://we.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ea.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://hx.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bg.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vv.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://db.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://lv.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ew.haigaiapp.cn

[C02] 默认参数
来源：http://ix.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://lo.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ho.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://gs.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rp.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fw.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xq.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://of.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://qw.yuexingan06.cn

[C03] 可变参数
来源：http://hy.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://ym.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zs.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wo.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cv.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fm.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aw.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gr.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cq.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://zi.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tz.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ag.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ud.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hw.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://on.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://he.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://ol.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://ou.bjjhwx.cn

[C05] 返回多个值
来源：http://lj.yuexingan06.cn

Py:   return a, b
来源：http://mf.nszjky.cn

PHP:  return [$a, $b];
来源：http://ay.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://km.bjjhwx.cn

TS:   return { a, b };
来源：http://uq.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nu.shtwfgs.cn

Go:   return a, b
来源：http://th.9csxet.cn

Ruby: return a, b
来源：http://fr.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://gp.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://ji.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://ku.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fk.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://mc.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://vk.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ft.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://es.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://zd.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kx.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://ti.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vp.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gm.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ld.nicolike.cn

TS:   arr.map(String)
来源：http://la.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://di.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tz.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://nz.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kv.bjjhwx.cn

[C08] 闭包
来源：http://kw.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tx.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pk.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rd.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yo.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cj.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qd.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kx.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gf.wgjwhj.cn

[C09] 递归
来源：http://ir.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qq.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bv.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ah.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ad.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xh.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wq.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nl.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xk.shxzukj.cn

[C10] 变量作用域
来源：http://ee.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iv.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ie.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uy.huanxung.cn

TS:   同 JS
来源：http://za.521024.cn

Java: 方法内为块级作用域
来源：http://sw.shtwfgs.cn

Go:   花括号块级作用域
来源：http://zc.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fy.colortex.cn

C#:   块级作用域
来源：http://wo.521024.cn

[C11] 模块导入与导出
来源：http://ye.szxytkj.cn

Py:   from module import func
来源：http://cz.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vy.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rc.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yd.bookmarksfly.cn

Java: import java.util.List;
来源：http://ru.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kr.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://vq.bjjhwx.cn

C#:   using System.Text;
来源：http://xp.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://qr.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://wn.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://qx.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://ap.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://xp.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ka.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://un.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://ds.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tk.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://yk.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xn.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dq.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://se.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dr.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://re.hnjuh.cn

Go:   func add(a, b int) int
来源：http://pf.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tl.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cl.asd995.cn

[C14] 泛型函数
来源：http://rz.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://je.yuexingan06.cn

PHP:  // 无泛型
来源：http://js.nszjky.cn

JS:   // 无泛型
来源：http://nw.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gc.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yt.szxytkj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://db.lnxyls.cn

Ruby: # 无泛型
来源：http://jn.shtwfgs.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qo.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://se.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://us.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://bi.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pw.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yp.bjjhwx.cn

Java: // 无解构
来源：http://bn.yuntaijiaju.cn

Go:   // 无解构
来源：http://ou.nicolike.cn

Ruby: a, b = pair
来源：http://in.9csxet.cn

C#:   var (a, b) = pair;
来源：http://ie.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://kf.chemitech.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tw.jianghongdianzi.cn

PHP:  // 无重载
来源：http://zp.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yr.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://pk.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sw.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://fd.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://dh.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rb.panjiajie.cn

================================================================================
来源：http://wq.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://tg.shtwfgs.cn

================================================================================
来源：http://lh.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://cu.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vj.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wt.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ju.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zm.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zl.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://qv.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://vu.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xe.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://zr.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dv.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yy.gzmigu.cn

JS:   arr.push(4);
来源：http://lc.haigaiapp.cn

TS:   arr.push(4);
来源：http://ip.asd995.cn

Java: list.add(4);
来源：http://yh.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://ly.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://pb.newstarts.cn

C#:   list.Add(4);
来源：http://hj.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://wb.521024.cn

Py:   arr.insert(0, 0)
来源：http://if.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xh.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xi.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ed.asd995.cn

Java: list.add(0, 0);
来源：http://om.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kj.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jh.shxzskj.cn

C#:   list.Insert(0, 0);
来源：http://ic.newstarts.cn

[D04] 删除元素
来源：http://uj.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sq.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vv.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jw.521024.cn

TS:   arr.splice(0, 1);
来源：http://bk.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bp.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pc.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://el.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ja.gzmigu.cn

[D05] 访问与修改元素
来源：http://zh.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ci.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wa.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ae.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://ld.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://au.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://be.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mu.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qv.bookmarksfly.cn

[D06] 数组长度
来源：http://no.szsharing.cn

Py:   len(arr)
来源：http://yw.colortex.cn

PHP:  count($arr);
来源：http://yu.lnxyls.cn

JS:   arr.length
来源：http://zn.bookmarksfly.cn

TS:   arr.length
来源：http://pk.haigaiapp.cn

Java: list.size();
来源：http://mh.szsharing.cn

Go:   len(arr)
来源：http://jo.huanxung.cn

Ruby: arr.length; arr.size
来源：http://ah.9csxet.cn

C#:   list.Count;
来源：http://lx.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://qg.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cb.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ak.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://nk.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://je.newstarts.cn

Java: list.subList(1, 4);
来源：http://xp.nicolike.cn

Go:   arr[1:4]
来源：http://cz.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://ng.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://mv.jctech888.com.cn

[D08] 合并两个数组
来源：http://zh.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://wc.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://ps.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dm.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://pd.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eq.lnxyls.cn

Go:   append(a, b...)
来源：http://mh.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://ie.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://ve.gzmigu.cn

[D09] 排序（升序）
来源：http://en.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ys.bookmarksfly.cn

PHP:  sort($arr);
来源：http://hw.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sj.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ft.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dt.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nn.9csxet.cn

Ruby: arr.sort
来源：http://ft.shxzskj.cn

C#:   list.Sort();
来源：http://jf.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hk.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sx.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kc.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uj.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vq.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eu.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iz.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pe.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pl.shtwfgs.cn

[D11] 反转数组
来源：http://ob.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://as.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://zm.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yt.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://wo.9csxet.cn

Java: Collections.reverse(list);
来源：http://qp.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://uh.521024.cn

Ruby: arr.reverse
来源：http://fc.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://xk.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://ua.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://ed.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vx.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nk.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xp.nszjky.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://oc.hnjuh.cn

Ruby: arr.index(x)
来源：http://fy.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://ql.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://cm.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ln.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ww.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://xa.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://bd.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fx.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lp.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pd.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rj.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://hn.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://er.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fm.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://sx.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://hy.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://la.yuntaijiaju.cn

Go:   // 手写循环
来源：http://so.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lm.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lq.yuexingan06.cn

[D15] 去重
来源：http://wb.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cz.hahajie.cn

PHP:  array_unique($arr);
来源：http://mh.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://yh.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://ut.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fh.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://os.huixiangedu.cn

Ruby: arr.uniq
来源：http://qo.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://yt.wgjwhj.cn

[D16] 求和与平均值
来源：http://fp.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rq.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ah.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kk.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aa.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iy.bjjhwx.cn

Go:   // 手写循环累加
来源：http://qw.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nd.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://rg.shxzskj.cn

[D17] 最大值与最小值
来源：http://nf.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://bc.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://cv.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://md.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://xt.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kh.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://im.nicolike.cn

Ruby: arr.max;  arr.min
来源：http://qe.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://qf.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://bh.gzmigu.cn


<!-- 参考信息 -->