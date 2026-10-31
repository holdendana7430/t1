代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://by.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vj.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ww.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ze.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wb.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wm.shxzukj.cn

[C04] 命名参数 / 关键字参数
来源：http://no.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pe.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nb.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vq.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zo.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://cm.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://bl.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://mn.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://ge.huixinmuqiang.cn

[C05] 返回多个值
来源：http://xz.bookmarksfly.cn

Py:   return a, b
来源：http://ng.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://rj.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nv.newstarts.cn

TS:   return { a, b };
来源：http://nt.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wh.gzmigu.cn

Go:   return a, b
来源：http://zk.huanxung.cn

Ruby: return a, b
来源：http://pl.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://wd.colortex.cn

[C06] 匿名函数 / lambda
来源：http://kp.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://hg.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://eu.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://mp.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://xp.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qn.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jl.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://pg.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hh.huanxung.cn

[C07] 把函数作为参数传入
来源：http://sl.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yo.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://eo.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bt.newstarts.cn

TS:   arr.map(String)
来源：http://la.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gx.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gm.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://ai.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jg.jctech888.com.cn

[C08] 闭包
来源：http://dk.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vh.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iz.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hf.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wv.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vf.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fp.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://px.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sp.panjiajie.cn

[C09] 递归
来源：http://hx.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xg.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pa.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jy.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://am.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nx.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jj.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zp.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ap.muxihuayi.cn

[C10] 变量作用域
来源：http://yn.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qh.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yh.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://de.521024.cn

TS:   同 JS
来源：http://fa.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://xa.wgjwhj.cn

Go:   花括号块级作用域
来源：http://ds.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rp.521024.cn

C#:   块级作用域
来源：http://ua.huanxung.cn

[C11] 模块导入与导出
来源：http://hk.jctech888.com.cn

Py:   from module import func
来源：http://fb.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rq.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zo.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://us.shxzukj.cn

Java: import java.util.List;
来源：http://eo.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mi.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://cm.chemitech.net.cn

C#:   using System.Text;
来源：http://zt.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://gu.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://ww.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://mr.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://li.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://uv.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kk.9csxet.cn

Go:   func() { fmt.Println("run") }()
来源：http://fr.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://pi.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jo.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://im.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sl.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lx.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bc.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vw.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wy.gzmigu.cn

Go:   func add(a, b int) int
来源：http://tp.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fs.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hv.haigaiapp.cn

[C14] 泛型函数
来源：http://xk.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gl.nszjky.cn

PHP:  // 无泛型
来源：http://ds.huixiangedu.cn

JS:   // 无泛型
来源：http://ea.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://an.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hk.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jn.hahajie.cn

Ruby: # 无泛型
来源：http://bd.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://py.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://fc.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tn.9csxet.cn

PHP:  [$a, $b] = $pair;
来源：http://zk.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jn.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bm.yuntaijiaju.cn

Java: // 无解构
来源：http://vd.wgjwhj.cn

Go:   // 无解构
来源：http://zn.panjiajie.cn

Ruby: a, b = pair
来源：http://sa.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://ch.nicolike.cn

[C16] 函数 / 方法重载
来源：http://ze.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jl.bookmarksfly.cn

PHP:  // 无重载
来源：http://yt.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ni.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://ta.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oc.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://vy.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://dz.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tg.muxihuayi.cn

================================================================================
来源：http://lf.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://ne.muxihuayi.cn

================================================================================
来源：http://lu.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://ct.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kv.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kp.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sd.szxytkj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lc.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gg.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://kc.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://yz.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wj.hnjuh.cn

[D02] 追加元素到末尾
来源：http://hj.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eb.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qz.nicolike.cn

JS:   arr.push(4);
来源：http://ed.haigaiapp.cn

TS:   arr.push(4);
来源：http://nm.nicolike.cn

Java: list.add(4);
来源：http://fs.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://li.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://sy.shtwfgs.cn

C#:   list.Add(4);
来源：http://nd.colortex.cn

[D03] 在指定位置插入元素
来源：http://fe.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://xp.lnxyls.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vu.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xf.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://jh.9csxet.cn

Java: list.add(0, 0);
来源：http://yw.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ax.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dk.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://xh.bjjhwx.cn

[D04] 删除元素
来源：http://xj.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fc.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lj.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qv.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://sp.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://px.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xp.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zr.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zv.shxzskj.cn

[D05] 访问与修改元素
来源：http://ch.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ee.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://po.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mw.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://yn.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://wh.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://dd.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mb.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aw.jctech888.com.cn

[D06] 数组长度
来源：http://ie.huixinmuqiang.cn

Py:   len(arr)
来源：http://uv.gzmigu.cn

PHP:  count($arr);
来源：http://cn.szsharing.cn

JS:   arr.length
来源：http://sf.yuexingan06.cn

TS:   arr.length
来源：http://ti.chemitech.net.cn

Java: list.size();
来源：http://be.hnjuh.cn

Go:   len(arr)
来源：http://ic.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://it.hnjuh.cn

C#:   list.Count;
来源：http://nh.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://sr.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://up.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oo.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://jo.521024.cn

TS:   arr.slice(1, 4);
来源：http://bs.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://jb.hahajie.cn

Go:   arr[1:4]
来源：http://si.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://xk.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://ka.shxzskj.cn

[D08] 合并两个数组
来源：http://gq.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://vs.asd995.cn

PHP:  array_merge($a, $b);
来源：http://nq.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://to.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://mz.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://my.nicolike.cn

Go:   append(a, b...)
来源：http://zn.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://or.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://lc.panjiajie.cn

[D09] 排序（升序）
来源：http://kq.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ty.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://sk.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hw.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iy.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tp.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://in.lnxyls.cn

Ruby: arr.sort
来源：http://je.hahajie.cn

C#:   list.Sort();
来源：http://wu.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rh.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rl.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lw.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wn.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://km.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nl.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xi.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://it.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qi.szsharing.cn

[D11] 反转数组
来源：http://nv.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ig.nicolike.cn

PHP:  array_reverse($arr);
来源：http://aj.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cc.nszjky.cn

TS:   [...arr].reverse();
来源：http://rb.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://wm.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://ac.szxytkj.cn

Ruby: arr.reverse
来源：http://lw.newstarts.cn

C#:   list.Reverse();
来源：http://qi.muxihuayi.cn

[D12] 查找元素下标
来源：http://de.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://ez.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kx.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hd.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gr.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qj.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://ja.chemitech.net.cn

Ruby: arr.index(x)
来源：http://zq.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://kd.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://qv.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hm.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pf.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://ax.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://jm.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oi.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pe.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://eb.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lk.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://fl.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jq.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cq.521024.cn

JS:   arr.map(x => x * 2)
来源：http://nh.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://xc.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ng.jctech888.com.cn

Go:   // 手写循环
来源：http://qo.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nv.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qh.asd995.cn

[D15] 去重
来源：http://un.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zm.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://xw.hahajie.cn

JS:   [...new Set(arr)]
来源：http://ti.hahajie.cn

TS:   [...new Set(arr)]
来源：http://cz.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yu.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rf.asd995.cn

Ruby: arr.uniq
来源：http://tk.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://ss.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://qa.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lm.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vf.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fa.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qc.wgjwhj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hy.hnjuh.cn

Go:   // 手写循环累加
来源：http://uk.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gv.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://jj.bjjhwx.cn

[D17] 最大值与最小值
来源：http://ec.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://dn.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://uw.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vf.shxzukj.cn

TS:   Math.max(...arr);
来源：http://xp.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sl.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uq.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://vd.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://mj.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://tp.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aa.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://hv.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ao.yuexingan06.cn

TS:   nested.flat();
来源：http://nr.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vw.521024.cn

Go:   // 手写双层循环
来源：http://wd.muxihuayi.cn

Ruby: nested.flatten
来源：http://yy.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wn.jianghongdianzi.cn

[D19] 按字段分组
来源：http://uv.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qe.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gd.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gy.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xx.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jo.szxytkj.cn

Go:   // 手写 map[string][]T
来源：http://vq.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dc.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oq.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://ym.szsharing.cn

Py:   Counter(arr)
来源：http://rv.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://of.jctech888.com.cn


<!-- 参考信息 -->