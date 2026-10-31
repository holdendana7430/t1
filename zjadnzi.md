代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://gq.haigaiapp.cn

[C03] 可变参数
来源：http://sl.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://ko.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rb.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jd.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dr.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qu.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mh.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cq.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ms.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://qw.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sm.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qw.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cv.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://py.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://tx.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://nj.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://ut.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://tl.bjjhwx.cn

[C05] 返回多个值
来源：http://yw.yuntaijiaju.cn

Py:   return a, b
来源：http://so.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://qi.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cj.nszjky.cn

TS:   return { a, b };
来源：http://vo.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qs.szxytkj.cn

Go:   return a, b
来源：http://hs.jctech888.com.cn

Ruby: return a, b
来源：http://hs.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://eu.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://of.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://hf.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zm.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://wa.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://dw.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yq.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qs.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://fb.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hu.9csxet.cn

[C07] 把函数作为参数传入
来源：http://gb.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tb.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ny.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://un.huanxung.cn

TS:   arr.map(String)
来源：http://dg.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kg.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pp.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://my.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hj.lnxyls.cn

[C08] 闭包
来源：http://em.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zs.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qa.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kj.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jg.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hw.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dg.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sp.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sn.yuexingan06.cn

[C09] 递归
来源：http://bp.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dn.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hp.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kw.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pz.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ii.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xl.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://js.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rn.521024.cn

[C10] 变量作用域
来源：http://ky.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://no.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hd.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xg.bjjhwx.cn

TS:   同 JS
来源：http://jb.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://ee.521024.cn

Go:   花括号块级作用域
来源：http://nz.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yu.yuntaijiaju.cn

C#:   块级作用域
来源：http://og.newstarts.cn

[C11] 模块导入与导出
来源：http://cc.muxihuayi.cn

Py:   from module import func
来源：http://lv.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wy.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://am.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qw.shtwfgs.cn

Java: import java.util.List;
来源：http://gr.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uh.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://uq.wgjwhj.cn

C#:   using System.Text;
来源：http://fo.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://im.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://xw.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://ok.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://ql.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://ao.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fg.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://qn.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://zc.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nt.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://cl.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xi.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bn.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nf.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wh.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ka.gzmigu.cn

Go:   func add(a, b int) int
来源：http://px.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qt.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zj.521024.cn

[C14] 泛型函数
来源：http://yo.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://be.muxihuayi.cn

PHP:  // 无泛型
来源：http://bl.huixiangedu.cn

JS:   // 无泛型
来源：http://qc.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xd.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://it.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://si.bjjhwx.cn

Ruby: # 无泛型
来源：http://dh.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mx.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://jj.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hu.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://mr.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oz.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pw.colortex.cn

Java: // 无解构
来源：http://qi.huanxung.cn

Go:   // 无解构
来源：http://zp.lnxyls.cn

Ruby: a, b = pair
来源：http://kp.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://sh.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://vi.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jq.bookmarksfly.cn

PHP:  // 无重载
来源：http://eb.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mt.huixinmuqiang.cn

TS:   // 用联合类型或重载签名声明
来源：http://ap.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://il.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://ji.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://rx.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ci.yuntaijiaju.cn

================================================================================
来源：http://pe.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://xe.yuntaijiaju.cn

================================================================================
来源：http://db.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://ja.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ju.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xc.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xu.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qd.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ds.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://fe.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://fy.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ij.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://dk.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ho.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kc.hnjuh.cn

JS:   arr.push(4);
来源：http://yr.521024.cn

TS:   arr.push(4);
来源：http://ji.szsharing.cn

Java: list.add(4);
来源：http://za.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://cl.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://gh.gzmigu.cn

C#:   list.Add(4);
来源：http://pt.9csxet.cn

[D03] 在指定位置插入元素
来源：http://ao.521024.cn

Py:   arr.insert(0, 0)
来源：http://zb.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wf.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pc.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://gv.panjiajie.cn

Java: list.add(0, 0);
来源：http://eg.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ni.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://og.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://lc.wgjwhj.cn

[D04] 删除元素
来源：http://tb.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qc.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ml.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ki.colortex.cn

TS:   arr.splice(0, 1);
来源：http://jg.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://la.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jh.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nt.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eq.chemitech.net.cn

[D05] 访问与修改元素
来源：http://gh.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ge.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ss.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xu.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://pt.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://qo.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://af.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nh.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sc.lnxyls.cn

[D06] 数组长度
来源：http://aa.muxihuayi.cn

Py:   len(arr)
来源：http://js.szsharing.cn

PHP:  count($arr);
来源：http://lw.muxihuayi.cn

JS:   arr.length
来源：http://ze.9csxet.cn

TS:   arr.length
来源：http://lf.huixinmuqiang.cn

Java: list.size();
来源：http://rf.hahajie.cn

Go:   len(arr)
来源：http://zo.shxzukj.cn

Ruby: arr.length; arr.size
来源：http://ab.jianghongdianzi.cn

C#:   list.Count;
来源：http://wv.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://hl.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tp.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://by.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://os.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://gd.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://kl.wgjwhj.cn

Go:   arr[1:4]
来源：http://es.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://ev.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://ao.haigaiapp.cn

[D08] 合并两个数组
来源：http://fq.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://bx.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://tw.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bz.bjjhwx.cn

TS:   [...a, ...b];
来源：http://jy.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vd.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://zj.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://xa.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://jy.szxytkj.cn

[D09] 排序（升序）
来源：http://qf.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://du.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://sy.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rq.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ha.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bt.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://of.hnjuh.cn

Ruby: arr.sort
来源：http://sx.shxzukj.cn

C#:   list.Sort();
来源：http://sa.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wc.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xj.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://be.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hb.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jv.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sk.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fx.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gs.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uv.haigaiapp.cn

[D11] 反转数组
来源：http://um.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xj.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://rb.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wd.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://ed.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://gb.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://sk.newstarts.cn

Ruby: arr.reverse
来源：http://dp.shxzukj.cn

C#:   list.Reverse();
来源：http://zx.szsharing.cn

[D12] 查找元素下标
来源：http://vy.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://gg.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hk.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yz.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kq.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bv.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://ic.chemitech.net.cn

Ruby: arr.index(x)
来源：http://zu.huanxung.cn

C#:   list.IndexOf(x);
来源：http://qo.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://iy.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ej.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xj.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://cp.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://vs.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zc.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xf.chemitech.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ik.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ua.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://jj.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ql.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ba.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://vy.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://ol.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dk.bjjhwx.cn

Go:   // 手写循环
来源：http://rf.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ru.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ff.huanxung.cn

[D15] 去重
来源：http://qr.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sq.asd995.cn

PHP:  array_unique($arr);
来源：http://fr.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://qc.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://ug.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ww.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mx.nszjky.cn

Ruby: arr.uniq
来源：http://ec.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://ii.bjjhwx.cn

[D16] 求和与平均值
来源：http://iz.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ai.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gi.nicolike.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://az.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lb.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xf.panjiajie.cn

Go:   // 手写循环累加
来源：http://my.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jy.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://go.colortex.cn

[D17] 最大值与最小值
来源：http://ne.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://ga.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://fm.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kx.szxytkj.cn

TS:   Math.max(...arr);
来源：http://wi.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ht.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ae.huixinmuqiang.cn

Ruby: arr.max;  arr.min
来源：http://ya.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://af.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://rw.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://am.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://qw.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ff.gzmigu.cn

TS:   nested.flat();
来源：http://cg.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kc.huanxung.cn

Go:   // 手写双层循环
来源：http://lt.nszjky.cn

Ruby: nested.flatten
来源：http://ck.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gw.gzmigu.cn

[D19] 按字段分组
来源：http://ca.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hy.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yt.colortex.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ci.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wb.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lp.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://in.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kk.yuntaijiaju.cn


<!-- 参考信息 -->