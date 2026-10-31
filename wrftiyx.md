代发 wailian999

Py:   if not data: return
来源：http://ki.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://hw.asd995.cn

JS:   if (!data) return;
来源：http://ui.muxihuayi.cn

TS:   if (!data) return;
来源：http://lg.jctech888.com.cn

Java: if (data == null) return;
来源：http://nv.shxzskj.cn

Go:   if data == nil { return }
来源：http://og.hnjuh.cn

Ruby: return if data.nil?
来源：http://rt.muxihuayi.cn

C#:   if (data == null) return;
来源：http://bc.yuntaijiaju.cn

================================================================================
来源：http://az.bjjhwx.cn

C. 函数与作用域
来源：http://rz.lnxyls.cn

================================================================================
来源：http://zx.nicolike.cn

[C01] 定义函数
来源：http://xb.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://pe.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qh.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://cv.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://je.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dq.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ub.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://wr.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oo.gzmigu.cn

[C02] 默认参数
来源：http://vn.521024.cn

Py:   def greet(name="World"): return name
来源：http://lg.bookmarksfly.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mb.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://yb.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nw.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nt.nszjky.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kt.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://qn.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ru.yuexingan06.cn

[C03] 可变参数
来源：http://fa.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://ol.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ua.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cv.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yz.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qp.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://th.szxytkj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gg.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cp.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://de.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uo.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tn.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pb.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wd.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://zt.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://qs.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://tg.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://em.huixinmuqiang.cn

[C05] 返回多个值
来源：http://lg.wgjwhj.cn

Py:   return a, b
来源：http://mz.huanxung.cn

PHP:  return [$a, $b];
来源：http://ty.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fs.shxzskj.cn

TS:   return { a, b };
来源：http://he.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hw.muxihuayi.cn

Go:   return a, b
来源：http://ho.panjiajie.cn

Ruby: return a, b
来源：http://ur.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://wi.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://mg.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://bd.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gs.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://zr.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://qx.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ya.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://em.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://qs.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://at.hahajie.cn

[C07] 把函数作为参数传入
来源：http://si.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yk.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tl.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wd.szxytkj.cn

TS:   arr.map(String)
来源：http://yy.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://st.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zr.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://iq.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ez.gzmigu.cn

[C08] 闭包
来源：http://zl.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wm.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ac.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wy.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hh.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gh.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wx.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gs.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://by.9csxet.cn

[C09] 递归
来源：http://xj.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kf.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pw.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rw.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iu.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ul.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hw.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ln.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qi.colortex.cn

[C10] 变量作用域
来源：http://ed.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eq.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ed.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cw.wgjwhj.cn

TS:   同 JS
来源：http://ol.nszjky.cn

Java: 方法内为块级作用域
来源：http://nk.szxytkj.cn

Go:   花括号块级作用域
来源：http://pl.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ys.nicolike.cn

C#:   块级作用域
来源：http://yt.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://vc.chemitech.net.cn

Py:   from module import func
来源：http://lp.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rx.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://my.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xf.szsharing.cn

Java: import java.util.List;
来源：http://by.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gb.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://jx.haigaiapp.cn

C#:   using System.Text;
来源：http://iv.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://nu.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://pe.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://pc.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://yo.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://cs.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kj.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://ka.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://wm.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gs.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://vp.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ts.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://li.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lw.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pj.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://da.szxytkj.cn

Go:   func add(a, b int) int
来源：http://cq.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://at.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ls.szxytkj.cn

[C14] 泛型函数
来源：http://yn.asd995.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ri.muxihuayi.cn

PHP:  // 无泛型
来源：http://hf.panjiajie.cn

JS:   // 无泛型
来源：http://xc.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tx.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ft.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xw.asd995.cn

Ruby: # 无泛型
来源：http://kk.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iw.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://np.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ar.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://go.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cj.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ph.jianghongdianzi.cn

Java: // 无解构
来源：http://sc.hnjuh.cn

Go:   // 无解构
来源：http://mp.muxihuayi.cn

Ruby: a, b = pair
来源：http://cn.521024.cn

C#:   var (a, b) = pair;
来源：http://qx.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://vq.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qt.nszjky.cn

PHP:  // 无重载
来源：http://tm.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ln.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://lw.huixiangedu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vp.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://yh.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://tl.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://si.yuntaijiaju.cn

================================================================================
来源：http://uh.lnxyls.cn

D. 数组 / 列表 / 集合
来源：http://ut.muxihuayi.cn

================================================================================
来源：http://vl.newstarts.cn

[D01] 创建数组 / 列表
来源：http://ts.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dj.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ba.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pf.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xn.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dt.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://sa.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://nl.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ge.gzmigu.cn

[D02] 追加元素到末尾
来源：http://vx.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uz.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sz.szsharing.cn

JS:   arr.push(4);
来源：http://zq.huanxung.cn

TS:   arr.push(4);
来源：http://nu.panjiajie.cn

Java: list.add(4);
来源：http://jd.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://to.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://qt.yuexingan06.cn

C#:   list.Add(4);
来源：http://zj.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://ru.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://jj.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rl.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lm.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://qh.huanxung.cn

Java: list.add(0, 0);
来源：http://rb.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gn.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ku.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://yf.huixiangedu.cn

[D04] 删除元素
来源：http://hz.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://an.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ou.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kg.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://dw.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gz.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cw.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bd.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ad.szsharing.cn

[D05] 访问与修改元素
来源：http://en.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lj.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yy.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lm.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://xe.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://ob.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ss.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gl.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://en.szxytkj.cn

[D06] 数组长度
来源：http://zk.bookmarksfly.cn

Py:   len(arr)
来源：http://ap.bjjhwx.cn

PHP:  count($arr);
来源：http://sr.colortex.cn

JS:   arr.length
来源：http://ef.shtwfgs.cn

TS:   arr.length
来源：http://cv.yuntaijiaju.cn

Java: list.size();
来源：http://li.asd995.cn

Go:   len(arr)
来源：http://ih.colortex.cn

Ruby: arr.length; arr.size
来源：http://ce.szsharing.cn

C#:   list.Count;
来源：http://wh.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://ab.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oj.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pp.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://ld.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://my.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://ad.bookmarksfly.cn

Go:   arr[1:4]
来源：http://rx.9csxet.cn

Ruby: arr[1, 3]
来源：http://nv.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://if.bookmarksfly.cn

[D08] 合并两个数组
来源：http://li.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://oh.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://bv.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jp.yuexingan06.cn

TS:   [...a, ...b];
来源：http://dq.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gz.521024.cn

Go:   append(a, b...)
来源：http://dt.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://kq.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://lk.szxytkj.cn

[D09] 排序（升序）
来源：http://pa.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://im.huanxung.cn

PHP:  sort($arr);
来源：http://oc.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cr.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ni.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://li.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://br.lnxyls.cn

Ruby: arr.sort
来源：http://nc.wgjwhj.cn

C#:   list.Sort();
来源：http://ya.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://aj.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ac.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lx.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nq.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ng.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bn.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sz.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gk.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bj.nszjky.cn

[D11] 反转数组
来源：http://fl.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hc.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://ly.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bj.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://cr.9csxet.cn

Java: Collections.reverse(list);
来源：http://oh.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://oq.bookmarksfly.cn

Ruby: arr.reverse
来源：http://dx.521024.cn

C#:   list.Reverse();
来源：http://um.colortex.cn

[D12] 查找元素下标
来源：http://np.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://pk.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kc.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hv.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fz.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ac.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://vr.huixiangedu.cn

Ruby: arr.index(x)
来源：http://th.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://nw.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://ge.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://un.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hb.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://km.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://wq.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dv.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ku.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fn.haigaiapp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ih.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://qj.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hu.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://su.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://my.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://ue.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rk.newstarts.cn

Go:   // 手写循环
来源：http://lp.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hu.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sc.szxytkj.cn

[D15] 去重
来源：http://gg.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oj.asd995.cn

PHP:  array_unique($arr);
来源：http://bg.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://pb.colortex.cn

TS:   [...new Set(arr)]
来源：http://ao.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vs.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rq.muxihuayi.cn

Ruby: arr.uniq
来源：http://kg.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://gg.bookmarksfly.cn

[D16] 求和与平均值
来源：http://vw.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://id.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://by.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tl.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pj.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pg.gzmigu.cn

Go:   // 手写循环累加
来源：http://xn.521024.cn


<!-- 参考信息 -->