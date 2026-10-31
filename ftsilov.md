代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://hn.9csxet.cn

[C03] 可变参数
来源：http://ds.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://jh.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://je.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lv.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hi.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wf.szsharing.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ms.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ui.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://af.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://er.jctech888.com.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tk.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ei.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oa.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://id.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://kd.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://ls.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://lh.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://hp.wgjwhj.cn

[C05] 返回多个值
来源：http://rx.shxzskj.cn

Py:   return a, b
来源：http://th.shxzskj.cn

PHP:  return [$a, $b];
来源：http://ex.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vs.huanxung.cn

TS:   return { a, b };
来源：http://yf.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eq.colortex.cn

Go:   return a, b
来源：http://gv.colortex.cn

Ruby: return a, b
来源：http://ki.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://cw.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://ed.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://wd.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wh.shxzskj.cn

JS:   const square = x => x * x;
来源：http://xn.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://dq.shxzukj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://br.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fn.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://cr.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xk.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://kv.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bk.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qg.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nk.wgjwhj.cn

TS:   arr.map(String)
来源：http://vz.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ni.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ch.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://zl.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yc.jctech888.com.cn

[C08] 闭包
来源：http://jv.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nu.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xj.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bb.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cn.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sg.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://io.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fa.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ra.haigaiapp.cn

[C09] 递归
来源：http://zc.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pk.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qp.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dx.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qq.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xk.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ty.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lf.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://aq.haigaiapp.cn

[C10] 变量作用域
来源：http://jd.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wf.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fk.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lp.lnxyls.cn

TS:   同 JS
来源：http://tt.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://cu.newstarts.cn

Go:   花括号块级作用域
来源：http://nl.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nh.bjjhwx.cn

C#:   块级作用域
来源：http://jx.huixiangedu.cn

[C11] 模块导入与导出
来源：http://tk.gzmigu.cn

Py:   from module import func
来源：http://cv.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nk.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vf.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zi.nicolike.cn

Java: import java.util.List;
来源：http://kh.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ap.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://be.shxzskj.cn

C#:   using System.Text;
来源：http://ct.huixiangedu.cn

[C12] 立即执行函数 IIFE
来源：http://im.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://vv.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://xs.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://fh.huixinmuqiang.cn

TS:   (() => { console.log("run"); })();
来源：http://mc.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lx.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://re.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://op.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zd.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://pi.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bs.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xr.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zb.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ae.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nj.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://et.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yf.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mg.huixiangedu.cn

[C14] 泛型函数
来源：http://zd.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bt.521024.cn

PHP:  // 无泛型
来源：http://iy.panjiajie.cn

JS:   // 无泛型
来源：http://ml.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jg.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pq.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vy.colortex.cn

Ruby: # 无泛型
来源：http://fu.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zh.huanxung.cn

[C15] 解构 / 展开参数
来源：http://iy.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yb.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://dx.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://og.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://np.huixiangedu.cn

Java: // 无解构
来源：http://fc.panjiajie.cn

Go:   // 无解构
来源：http://qk.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://un.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://va.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://we.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ay.nszjky.cn

PHP:  // 无重载
来源：http://tb.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://js.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://mf.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nn.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://xt.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://pu.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ak.colortex.cn

================================================================================
来源：http://za.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://la.muxihuayi.cn

================================================================================
来源：http://zx.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://pp.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dg.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wm.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lv.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uu.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cx.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://gu.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://wm.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vx.asd995.cn

[D02] 追加元素到末尾
来源：http://gy.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tk.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fc.bjjhwx.cn

JS:   arr.push(4);
来源：http://hs.yuexingan06.cn

TS:   arr.push(4);
来源：http://av.hahajie.cn

Java: list.add(4);
来源：http://bh.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://xg.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://em.yuexingan06.cn

C#:   list.Add(4);
来源：http://mf.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://vr.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://eo.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oa.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dc.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://tm.muxihuayi.cn

Java: list.add(0, 0);
来源：http://au.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mp.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://am.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://io.nszjky.cn

[D04] 删除元素
来源：http://xt.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ob.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gw.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pk.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://zt.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nt.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kw.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jn.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://co.shxzukj.cn

[D05] 访问与修改元素
来源：http://ij.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ji.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wq.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jz.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://jd.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://wg.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://wj.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vl.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yi.chemitech.net.cn

[D06] 数组长度
来源：http://me.szsharing.cn

Py:   len(arr)
来源：http://zw.bookmarksfly.cn

PHP:  count($arr);
来源：http://om.bjjhwx.cn

JS:   arr.length
来源：http://zk.panjiajie.cn

TS:   arr.length
来源：http://pu.szxytkj.cn

Java: list.size();
来源：http://hx.panjiajie.cn

Go:   len(arr)
来源：http://rs.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://my.yuntaijiaju.cn

C#:   list.Count;
来源：http://nn.huanxung.cn

[D07] 切片 / 取子数组
来源：http://io.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vc.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gw.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://hu.asd995.cn

TS:   arr.slice(1, 4);
来源：http://dx.colortex.cn

Java: list.subList(1, 4);
来源：http://sl.nszjky.cn

Go:   arr[1:4]
来源：http://jq.szsharing.cn

Ruby: arr[1, 3]
来源：http://ai.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://am.bjjhwx.cn

[D08] 合并两个数组
来源：http://fy.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://ch.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://fw.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://up.shxzskj.cn

TS:   [...a, ...b];
来源：http://uu.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wb.muxihuayi.cn

Go:   append(a, b...)
来源：http://zb.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://uf.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://yv.jctech888.com.cn

[D09] 排序（升序）
来源：http://gb.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://ws.bookmarksfly.cn

PHP:  sort($arr);
来源：http://tr.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sg.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pd.nszjky.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://eu.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ea.nicolike.cn

Ruby: arr.sort
来源：http://pn.yuntaijiaju.cn

C#:   list.Sort();
来源：http://fv.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hm.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ct.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zb.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tz.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://au.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://of.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ue.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fa.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qg.shxzskj.cn

[D11] 反转数组
来源：http://sx.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://do.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://hd.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jx.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://fg.szxytkj.cn

Java: Collections.reverse(list);
来源：http://yr.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://wu.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://xb.nszjky.cn

C#:   list.Reverse();
来源：http://il.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://hz.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://wc.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ov.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://et.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ck.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uh.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://ol.nszjky.cn

Ruby: arr.index(x)
来源：http://rg.nszjky.cn

C#:   list.IndexOf(x);
来源：http://yp.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://wr.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hm.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rl.wgjwhj.cn

JS:   arr.filter(x => x > 3)
来源：http://dt.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://qk.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://au.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yf.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://eb.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fj.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://yn.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rx.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ct.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://fl.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://ok.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xn.shxzukj.cn

Go:   // 手写循环
来源：http://ia.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://iq.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zf.newstarts.cn

[D15] 去重
来源：http://zz.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://or.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://sl.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://sb.newstarts.cn

TS:   [...new Set(arr)]
来源：http://ko.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zp.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tf.shxzskj.cn

Ruby: arr.uniq
来源：http://gg.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://fg.jctech888.com.cn

[D16] 求和与平均值
来源：http://bj.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fb.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tq.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://if.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gu.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ev.colortex.cn

Go:   // 手写循环累加
来源：http://oo.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xg.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://jp.asd995.cn

[D17] 最大值与最小值
来源：http://ea.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://cd.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://wn.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://me.hnjuh.cn

TS:   Math.max(...arr);
来源：http://cb.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xx.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jn.521024.cn

Ruby: arr.max;  arr.min
来源：http://rp.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://mb.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://uq.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uq.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://yo.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oa.szsharing.cn

TS:   nested.flat();
来源：http://nj.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dk.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://cx.haigaiapp.cn

Ruby: nested.flatten
来源：http://ws.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gh.hnjuh.cn

[D19] 按字段分组
来源：http://ph.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://er.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://od.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jj.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ji.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hj.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://kt.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xc.shtwfgs.cn


<!-- 参考信息 -->