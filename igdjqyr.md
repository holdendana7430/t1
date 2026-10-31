代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://fd.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ly.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://lo.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ht.huanxung.cn

[C02] 默认参数
来源：http://xu.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://lc.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qj.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://ah.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://az.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zn.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yk.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://bw.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://sq.521024.cn

[C03] 可变参数
来源：http://wb.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://rq.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mm.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qd.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vt.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gk.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zw.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wi.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dx.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://dq.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zo.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vy.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xm.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dv.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://qv.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://vs.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://wl.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://qy.nicolike.cn

[C05] 返回多个值
来源：http://pn.shxzukj.cn

Py:   return a, b
来源：http://ow.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://vv.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rb.hahajie.cn

TS:   return { a, b };
来源：http://la.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iu.muxihuayi.cn

Go:   return a, b
来源：http://xl.shtwfgs.cn

Ruby: return a, b
来源：http://ir.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://mg.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://uj.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://gu.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hp.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://ou.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://hj.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://az.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ts.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://si.nicolike.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jy.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://ie.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bi.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ub.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cv.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://gb.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cm.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ww.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://ua.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zi.colortex.cn

[C08] 闭包
来源：http://mm.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lb.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://va.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zw.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oq.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mh.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ew.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dx.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ro.haigaiapp.cn

[C09] 递归
来源：http://mw.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ui.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wi.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ju.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cm.yuexingan06.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oh.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://al.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://by.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yz.bookmarksfly.cn

[C10] 变量作用域
来源：http://dz.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cv.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://va.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://te.521024.cn

TS:   同 JS
来源：http://ut.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://rh.haigaiapp.cn

Go:   花括号块级作用域
来源：http://sj.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sy.panjiajie.cn

C#:   块级作用域
来源：http://lb.asd995.cn

[C11] 模块导入与导出
来源：http://ql.bookmarksfly.cn

Py:   from module import func
来源：http://bg.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qp.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gw.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jc.gzmigu.cn

Java: import java.util.List;
来源：http://za.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ha.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://fw.hnjuh.cn

C#:   using System.Text;
来源：http://om.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://qo.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://no.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://zl.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://cd.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://by.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ow.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://om.521024.cn

Ruby: -> { puts "run" }.call
来源：http://jk.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sh.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://hj.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://az.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cz.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mu.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ok.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yf.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://hp.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nw.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qh.yuexingan06.cn

[C14] 泛型函数
来源：http://xr.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ds.muxihuayi.cn

PHP:  // 无泛型
来源：http://ev.shxzskj.cn

JS:   // 无泛型
来源：http://xv.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ht.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://av.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://im.gzmigu.cn

Ruby: # 无泛型
来源：http://io.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gi.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://fi.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vb.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://os.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rf.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://av.haigaiapp.cn

Java: // 无解构
来源：http://bh.muxihuayi.cn

Go:   // 无解构
来源：http://sp.hnjuh.cn

Ruby: a, b = pair
来源：http://ch.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://rd.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://yr.chemitech.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ld.colortex.cn

PHP:  // 无重载
来源：http://yu.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rz.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://nj.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rb.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://gi.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://bb.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jz.9csxet.cn

================================================================================
来源：http://ya.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://tk.shxzskj.cn

================================================================================
来源：http://vs.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://jm.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://at.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mk.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iz.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ze.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ul.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://fz.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://de.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dc.9csxet.cn

[D02] 追加元素到末尾
来源：http://up.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qu.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uw.jctech888.com.cn

JS:   arr.push(4);
来源：http://yg.hahajie.cn

TS:   arr.push(4);
来源：http://vr.huixiangedu.cn

Java: list.add(4);
来源：http://cw.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://ss.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://ig.hahajie.cn

C#:   list.Add(4);
来源：http://mp.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://ga.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://mw.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gd.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ku.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://rh.huixiangedu.cn

Java: list.add(0, 0);
来源：http://ln.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fe.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dh.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://mc.jianghongdianzi.cn

[D04] 删除元素
来源：http://eh.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lu.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ax.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rl.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://pa.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yq.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xn.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://du.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fo.wgjwhj.cn

[D05] 访问与修改元素
来源：http://wt.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cf.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nz.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ye.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://eo.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://gg.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://pa.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ir.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kc.huixinmuqiang.cn

[D06] 数组长度
来源：http://gi.shxzskj.cn

Py:   len(arr)
来源：http://nb.newstarts.cn

PHP:  count($arr);
来源：http://yk.asd995.cn

JS:   arr.length
来源：http://ui.haigaiapp.cn

TS:   arr.length
来源：http://np.bookmarksfly.cn

Java: list.size();
来源：http://ht.nszjky.cn

Go:   len(arr)
来源：http://jt.newstarts.cn

Ruby: arr.length; arr.size
来源：http://ah.shtwfgs.cn

C#:   list.Count;
来源：http://kx.9csxet.cn

[D07] 切片 / 取子数组
来源：http://as.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fd.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jg.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://dz.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://bv.panjiajie.cn

Java: list.subList(1, 4);
来源：http://rp.colortex.cn

Go:   arr[1:4]
来源：http://vr.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://dw.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://gm.newstarts.cn

[D08] 合并两个数组
来源：http://zs.521024.cn

Py:   a + b;  a.extend(b)
来源：http://ib.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://eo.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ro.hnjuh.cn

TS:   [...a, ...b];
来源：http://be.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xg.shtwfgs.cn

Go:   append(a, b...)
来源：http://wz.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://zk.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://po.colortex.cn

[D09] 排序（升序）
来源：http://on.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://ra.jctech888.com.cn

PHP:  sort($arr);
来源：http://ex.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gt.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ld.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dh.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jh.bjjhwx.cn

Ruby: arr.sort
来源：http://ek.jctech888.com.cn

C#:   list.Sort();
来源：http://lt.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kc.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pl.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gq.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gd.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eu.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ox.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pe.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zv.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hd.chemitech.net.cn

[D11] 反转数组
来源：http://dv.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://te.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://yo.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mo.shxzskj.cn

TS:   [...arr].reverse();
来源：http://tl.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://hx.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://vs.9csxet.cn

Ruby: arr.reverse
来源：http://ly.colortex.cn

C#:   list.Reverse();
来源：http://kt.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://nb.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://um.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ns.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tj.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oq.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nc.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://jx.panjiajie.cn

Ruby: arr.index(x)
来源：http://fy.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://om.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://zy.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://av.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vi.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://fd.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://wq.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ue.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://su.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zj.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ws.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://gp.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sc.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fx.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://pp.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://ox.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jm.haigaiapp.cn

Go:   // 手写循环
来源：http://fg.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fr.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://es.jianghongdianzi.cn

[D15] 去重
来源：http://tx.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sa.lnxyls.cn

PHP:  array_unique($arr);
来源：http://zc.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://yj.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://ie.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://al.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zr.jctech888.com.cn

Ruby: arr.uniq
来源：http://sl.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://jx.jctech888.com.cn

[D16] 求和与平均值
来源：http://sw.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ty.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dc.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xm.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fm.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://su.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://bn.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mp.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://lv.muxihuayi.cn

[D17] 最大值与最小值
来源：http://uo.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://ia.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://eh.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://on.hnjuh.cn

TS:   Math.max(...arr);
来源：http://mk.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ks.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nl.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://ab.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://np.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://mx.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kz.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://wk.9csxet.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aj.chemitech.net.cn

TS:   nested.flat();
来源：http://hs.yuexingan06.cn


<!-- 参考信息 -->