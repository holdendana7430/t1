代发 wailian999

Py:   def add(a, b): return a + b
来源：http://mc.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xz.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://cu.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tq.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kk.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jk.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://lz.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zr.nszjky.cn

[C02] 默认参数
来源：http://oq.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://ia.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://eb.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://mz.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bv.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cq.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jf.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://ta.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://gl.shtwfgs.cn

[C03] 可变参数
来源：http://vs.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://ed.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yz.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qz.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cd.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://va.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yu.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fb.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yc.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://pb.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://el.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kr.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hm.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fn.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://xg.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://xl.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://wa.521024.cn

C#:   f(a: 1, b: 2)
来源：http://dv.9csxet.cn

[C05] 返回多个值
来源：http://lo.newstarts.cn

Py:   return a, b
来源：http://jo.9csxet.cn

PHP:  return [$a, $b];
来源：http://qb.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ps.shtwfgs.cn

TS:   return { a, b };
来源：http://ab.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://et.bookmarksfly.cn

Go:   return a, b
来源：http://ra.colortex.cn

Ruby: return a, b
来源：http://bu.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://rx.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://jr.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://dn.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ik.szsharing.cn

JS:   const square = x => x * x;
来源：http://im.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://ut.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xc.szsharing.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uy.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://ue.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rc.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://dt.yuexingan06.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nh.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vv.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xz.hnjuh.cn

TS:   arr.map(String)
来源：http://vn.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tc.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gs.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://nn.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vn.shtwfgs.cn

[C08] 闭包
来源：http://aa.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xq.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ms.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://um.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://la.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://av.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vq.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cz.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cn.asd995.cn

[C09] 递归
来源：http://ef.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://by.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gq.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jg.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hh.chemitech.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gf.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wa.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ky.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rd.gzmigu.cn

[C10] 变量作用域
来源：http://al.newstarts.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oz.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hm.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://as.hahajie.cn

TS:   同 JS
来源：http://ur.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://me.jctech888.com.cn

Go:   花括号块级作用域
来源：http://lc.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sp.colortex.cn

C#:   块级作用域
来源：http://df.hahajie.cn

[C11] 模块导入与导出
来源：http://qu.bookmarksfly.cn

Py:   from module import func
来源：http://tx.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rl.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kt.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xg.yuntaijiaju.cn

Java: import java.util.List;
来源：http://cn.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yp.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://ch.panjiajie.cn

C#:   using System.Text;
来源：http://cx.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://bd.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://vr.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://to.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://if.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://de.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lg.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://rz.521024.cn

Ruby: -> { puts "run" }.call
来源：http://yw.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://at.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://nf.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rk.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cu.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xa.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xe.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vt.szxytkj.cn

Go:   func add(a, b int) int
来源：http://ce.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dq.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ns.jianghongdianzi.cn

[C14] 泛型函数
来源：http://de.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://da.muxihuayi.cn

PHP:  // 无泛型
来源：http://vr.shtwfgs.cn

JS:   // 无泛型
来源：http://ek.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qy.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ap.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ec.lnxyls.cn

Ruby: # 无泛型
来源：http://ee.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://js.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://nx.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ey.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://of.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ng.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jg.yuexingan06.cn

Java: // 无解构
来源：http://wj.9csxet.cn

Go:   // 无解构
来源：http://ij.9csxet.cn

Ruby: a, b = pair
来源：http://lq.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://yb.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://bs.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ou.yuexingan06.cn

PHP:  // 无重载
来源：http://wx.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pn.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://xx.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qa.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://pw.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://zo.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://it.9csxet.cn

================================================================================
来源：http://ul.521024.cn

D. 数组 / 列表 / 集合
来源：http://hm.yuntaijiaju.cn

================================================================================
来源：http://iy.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://pj.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bs.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ov.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fp.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ai.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oq.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://uj.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://xe.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zw.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://il.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ib.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ja.hnjuh.cn

JS:   arr.push(4);
来源：http://hu.hahajie.cn

TS:   arr.push(4);
来源：http://zu.szxytkj.cn

Java: list.add(4);
来源：http://ys.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://qr.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://bv.bjjhwx.cn

C#:   list.Add(4);
来源：http://qr.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://pl.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://rb.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://be.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hn.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://ls.panjiajie.cn

Java: list.add(0, 0);
来源：http://hf.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nc.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qr.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://as.hahajie.cn

[D04] 删除元素
来源：http://ng.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tc.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zu.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cb.colortex.cn

TS:   arr.splice(0, 1);
来源：http://nf.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kf.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ys.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mv.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lx.panjiajie.cn

[D05] 访问与修改元素
来源：http://ip.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wo.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yz.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sy.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://jm.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://vq.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://qr.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ps.muxihuayi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vp.haigaiapp.cn

[D06] 数组长度
来源：http://sz.nszjky.cn

Py:   len(arr)
来源：http://un.shxzskj.cn

PHP:  count($arr);
来源：http://sx.gzmigu.cn

JS:   arr.length
来源：http://zn.panjiajie.cn

TS:   arr.length
来源：http://on.huixiangedu.cn

Java: list.size();
来源：http://nw.muxihuayi.cn

Go:   len(arr)
来源：http://kb.szsharing.cn

Ruby: arr.length; arr.size
来源：http://xt.szxytkj.cn

C#:   list.Count;
来源：http://xc.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://dd.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dk.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gp.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://zc.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://hn.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://ku.shxzskj.cn

Go:   arr[1:4]
来源：http://wq.shxzukj.cn

Ruby: arr[1, 3]
来源：http://qc.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://et.muxihuayi.cn

[D08] 合并两个数组
来源：http://eh.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://mb.asd995.cn

PHP:  array_merge($a, $b);
来源：http://js.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qt.shxzskj.cn

TS:   [...a, ...b];
来源：http://tx.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iz.jctech888.com.cn

Go:   append(a, b...)
来源：http://tm.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://pq.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://ev.szxytkj.cn

[D09] 排序（升序）
来源：http://jg.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://ri.asd995.cn

PHP:  sort($arr);
来源：http://pd.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bi.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vn.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ky.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cm.shxzskj.cn

Ruby: arr.sort
来源：http://uj.szsharing.cn

C#:   list.Sort();
来源：http://er.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rz.colortex.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ir.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fy.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sr.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hx.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gh.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bp.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ww.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://le.szsharing.cn

[D11] 反转数组
来源：http://yx.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qm.szsharing.cn

PHP:  array_reverse($arr);
来源：http://ov.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qb.521024.cn

TS:   [...arr].reverse();
来源：http://ax.szsharing.cn

Java: Collections.reverse(list);
来源：http://iv.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://wk.gzmigu.cn

Ruby: arr.reverse
来源：http://dj.bookmarksfly.cn

C#:   list.Reverse();
来源：http://tl.bjjhwx.cn

[D12] 查找元素下标
来源：http://bu.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://rw.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kl.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://an.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yh.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fc.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://sg.newstarts.cn

Ruby: arr.index(x)
来源：http://py.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://ax.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://it.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://je.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hy.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://vi.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://an.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://el.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dk.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ij.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rn.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://mc.nicolike.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bw.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uq.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://yj.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://te.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ih.yuntaijiaju.cn

Go:   // 手写循环
来源：http://vm.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wt.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://px.wgjwhj.cn

[D15] 去重
来源：http://rw.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ty.nszjky.cn

PHP:  array_unique($arr);
来源：http://wu.newstarts.cn

JS:   [...new Set(arr)]
来源：http://kk.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://cj.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jj.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qx.bookmarksfly.cn

Ruby: arr.uniq
来源：http://ig.colortex.cn

C#:   list.Distinct().ToList()
来源：http://kh.gzmigu.cn

[D16] 求和与平均值
来源：http://fx.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ry.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://is.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vd.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fp.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cw.panjiajie.cn

Go:   // 手写循环累加
来源：http://os.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ck.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://nd.huanxung.cn

[D17] 最大值与最小值
来源：http://dm.colortex.cn

Py:   max(arr);  min(arr)
来源：http://aw.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://fp.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.newstarts.cn

TS:   Math.max(...arr);
来源：http://wv.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wl.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xb.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://uv.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://rl.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://fl.szxytkj.cn


<!-- 参考信息 -->