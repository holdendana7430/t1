代发 wailian999

================================================================================
来源：http://rh.shxzskj.cn

C. 函数与作用域
来源：http://ls.yuntaijiaju.cn

================================================================================
来源：http://cb.szsharing.cn

[C01] 定义函数
来源：http://nc.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://mb.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qx.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://sy.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yz.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ux.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pq.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://cq.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yl.hnjuh.cn

[C02] 默认参数
来源：http://us.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://kb.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://li.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://pm.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nj.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qk.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://na.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://xn.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://gx.jianghongdianzi.cn

[C03] 可变参数
来源：http://kj.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://oy.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sp.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yx.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xl.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mk.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rg.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oo.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yr.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://wn.szxytkj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xc.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xk.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fg.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ql.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://qf.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://sx.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://br.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://bj.gzmigu.cn

[C05] 返回多个值
来源：http://jz.jianghongdianzi.cn

Py:   return a, b
来源：http://or.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://by.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ef.shtwfgs.cn

TS:   return { a, b };
来源：http://wr.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tr.jctech888.com.cn

Go:   return a, b
来源：http://rh.bookmarksfly.cn

Ruby: return a, b
来源：http://hy.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://gq.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://by.521024.cn

Py:   square = lambda x: x * x
来源：http://uy.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yf.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://mf.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://mr.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://at.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tw.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://pa.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qq.colortex.cn

[C07] 把函数作为参数传入
来源：http://ov.bookmarksfly.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bh.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ae.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fa.newstarts.cn

TS:   arr.map(String)
来源：http://cx.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ir.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://eb.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://lf.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mr.bjjhwx.cn

[C08] 闭包
来源：http://no.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ha.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rl.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://um.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://me.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hp.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rp.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ua.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://de.nszjky.cn

[C09] 递归
来源：http://uj.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xq.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gk.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oa.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ma.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://am.shxzskj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wu.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fl.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rf.shxzskj.cn

[C10] 变量作用域
来源：http://pl.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qf.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sa.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ne.bjjhwx.cn

TS:   同 JS
来源：http://uy.panjiajie.cn

Java: 方法内为块级作用域
来源：http://bw.colortex.cn

Go:   花括号块级作用域
来源：http://pi.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gl.huixiangedu.cn

C#:   块级作用域
来源：http://fa.szxytkj.cn

[C11] 模块导入与导出
来源：http://em.colortex.cn

Py:   from module import func
来源：http://qs.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ij.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://be.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fm.asd995.cn

Java: import java.util.List;
来源：http://mt.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qj.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://ct.jctech888.com.cn

C#:   using System.Text;
来源：http://hv.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://xh.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://db.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://fd.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://ol.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://ub.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xj.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://iu.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://iy.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ta.521024.cn

[C13] 类型声明 / 类型注解
来源：http://za.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tc.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hf.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uf.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gm.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://io.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://kq.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ij.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yj.nszjky.cn

[C14] 泛型函数
来源：http://ea.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ea.gzmigu.cn

PHP:  // 无泛型
来源：http://wd.huixiangedu.cn

JS:   // 无泛型
来源：http://ef.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vv.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vm.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sg.wgjwhj.cn

Ruby: # 无泛型
来源：http://qr.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jc.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://lj.yuntaijiaju.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yl.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://dc.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rm.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mc.huanxung.cn

Java: // 无解构
来源：http://dx.szxytkj.cn

Go:   // 无解构
来源：http://uk.muxihuayi.cn

Ruby: a, b = pair
来源：http://xo.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://pw.nszjky.cn

[C16] 函数 / 方法重载
来源：http://tl.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wx.huanxung.cn

PHP:  // 无重载
来源：http://oq.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ry.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://dn.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mg.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://cu.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://ux.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yf.shxzskj.cn

================================================================================
来源：http://yz.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://nr.nszjky.cn

================================================================================
来源：http://ab.newstarts.cn

[D01] 创建数组 / 列表
来源：http://ni.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yb.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ar.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gq.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sa.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hm.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://rt.yuexingan06.cn

Ruby: arr = [1, 2, 3]
来源：http://hm.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sa.hahajie.cn

[D02] 追加元素到末尾
来源：http://bd.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gj.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rw.521024.cn

JS:   arr.push(4);
来源：http://vl.nszjky.cn

TS:   arr.push(4);
来源：http://if.shxzukj.cn

Java: list.add(4);
来源：http://mg.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://fv.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://mg.gzmigu.cn

C#:   list.Add(4);
来源：http://ea.9csxet.cn

[D03] 在指定位置插入元素
来源：http://xm.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://hg.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zg.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zv.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://cs.huixiangedu.cn

Java: list.add(0, 0);
来源：http://mr.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pi.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://np.colortex.cn

C#:   list.Insert(0, 0);
来源：http://wx.nszjky.cn

[D04] 删除元素
来源：http://kr.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ga.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://su.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rc.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://wh.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yj.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dq.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ty.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xn.lnxyls.cn

[D05] 访问与修改元素
来源：http://ww.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ub.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gr.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vv.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://oa.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://dq.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://yn.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ci.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cn.521024.cn

[D06] 数组长度
来源：http://xo.colortex.cn

Py:   len(arr)
来源：http://vr.hnjuh.cn

PHP:  count($arr);
来源：http://lp.521024.cn

JS:   arr.length
来源：http://gc.huixiangedu.cn

TS:   arr.length
来源：http://cf.521024.cn

Java: list.size();
来源：http://ag.hnjuh.cn

Go:   len(arr)
来源：http://js.nszjky.cn

Ruby: arr.length; arr.size
来源：http://jz.szxytkj.cn

C#:   list.Count;
来源：http://hu.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://bb.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sk.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oe.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://qu.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://ln.szsharing.cn

Java: list.subList(1, 4);
来源：http://iq.huixiangedu.cn

Go:   arr[1:4]
来源：http://bn.gzmigu.cn

Ruby: arr[1, 3]
来源：http://on.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://ip.bjjhwx.cn

[D08] 合并两个数组
来源：http://cm.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://yh.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://zw.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gd.lnxyls.cn

TS:   [...a, ...b];
来源：http://iq.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jm.bjjhwx.cn

Go:   append(a, b...)
来源：http://zw.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://lf.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://ij.panjiajie.cn

[D09] 排序（升序）
来源：http://bm.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://le.shtwfgs.cn

PHP:  sort($arr);
来源：http://hl.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ll.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ft.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ks.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qa.shxzskj.cn

Ruby: arr.sort
来源：http://yl.lnxyls.cn

C#:   list.Sort();
来源：http://qn.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fn.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ju.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qc.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hw.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eg.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vd.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vt.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vs.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eh.jianghongdianzi.cn

[D11] 反转数组
来源：http://xl.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ii.szsharing.cn

PHP:  array_reverse($arr);
来源：http://qg.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ag.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://rf.lnxyls.cn

Java: Collections.reverse(list);
来源：http://cv.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://qz.yuexingan06.cn

Ruby: arr.reverse
来源：http://mg.jctech888.com.cn

C#:   list.Reverse();
来源：http://vn.muxihuayi.cn

[D12] 查找元素下标
来源：http://tl.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://rn.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jz.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xl.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iw.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hf.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://lz.shxzskj.cn

Ruby: arr.index(x)
来源：http://cm.521024.cn

C#:   list.IndexOf(x);
来源：http://bw.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://zv.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yc.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qf.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://kv.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://vx.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uw.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ov.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jh.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pv.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://bc.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://im.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fl.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://ku.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://ph.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cq.nicolike.cn

Go:   // 手写循环
来源：http://tb.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ay.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kz.jctech888.com.cn

[D15] 去重
来源：http://ym.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qz.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://gp.nicolike.cn

JS:   [...new Set(arr)]
来源：http://nn.hahajie.cn

TS:   [...new Set(arr)]
来源：http://uu.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hk.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://om.gzmigu.cn

Ruby: arr.uniq
来源：http://dv.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://re.lnxyls.cn

[D16] 求和与平均值
来源：http://rm.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fx.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ca.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nn.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mw.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fd.9csxet.cn

Go:   // 手写循环累加
来源：http://mt.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gs.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://uk.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://tr.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://qj.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://bh.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ir.colortex.cn

TS:   Math.max(...arr);
来源：http://ed.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zg.hnjuh.cn


<!-- 参考信息 -->