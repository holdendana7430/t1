代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://np.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://vu.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://ot.yuexingan06.cn

[C05] 返回多个值
来源：http://de.colortex.cn

Py:   return a, b
来源：http://sw.shxzskj.cn

PHP:  return [$a, $b];
来源：http://yn.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jx.shxzskj.cn

TS:   return { a, b };
来源：http://mk.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jr.521024.cn

Go:   return a, b
来源：http://jx.shtwfgs.cn

Ruby: return a, b
来源：http://sa.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://xf.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://za.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://vd.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lb.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://hh.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://ha.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://on.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hj.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://fb.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pj.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://ph.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://th.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wq.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ha.bjjhwx.cn

TS:   arr.map(String)
来源：http://ny.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dx.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://im.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://rt.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fi.huanxung.cn

[C08] 闭包
来源：http://fv.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ks.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lz.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yd.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vf.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ze.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tb.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ns.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rp.shtwfgs.cn

[C09] 递归
来源：http://ar.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wd.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uf.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://im.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zr.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://us.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ax.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iq.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://il.bjjhwx.cn

[C10] 变量作用域
来源：http://fy.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gm.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cl.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rh.bjjhwx.cn

TS:   同 JS
来源：http://do.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://wr.wgjwhj.cn

Go:   花括号块级作用域
来源：http://rb.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hn.hnjuh.cn

C#:   块级作用域
来源：http://hi.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://hw.hahajie.cn

Py:   from module import func
来源：http://je.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ux.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pb.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rb.szxytkj.cn

Java: import java.util.List;
来源：http://ud.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mh.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://ux.nszjky.cn

C#:   using System.Text;
来源：http://kn.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://ax.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://sf.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://bz.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://pa.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://de.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jw.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://it.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://ee.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ok.521024.cn

[C13] 类型声明 / 类型注解
来源：http://zr.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mt.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mc.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bl.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sj.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ga.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://op.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ak.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xi.bookmarksfly.cn

[C14] 泛型函数
来源：http://ex.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pi.wgjwhj.cn

PHP:  // 无泛型
来源：http://tq.shxzskj.cn

JS:   // 无泛型
来源：http://uj.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xb.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wj.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cr.panjiajie.cn

Ruby: # 无泛型
来源：http://ov.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bb.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://mr.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zf.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://hs.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qe.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://si.bjjhwx.cn

Java: // 无解构
来源：http://te.jctech888.com.cn

Go:   // 无解构
来源：http://qr.szsharing.cn

Ruby: a, b = pair
来源：http://ce.szsharing.cn

C#:   var (a, b) = pair;
来源：http://dx.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://rl.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qd.muxihuayi.cn

PHP:  // 无重载
来源：http://xw.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cm.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://hz.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pb.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://lr.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://mp.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yd.521024.cn

================================================================================
来源：http://eg.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://ba.shtwfgs.cn

================================================================================
来源：http://hm.9csxet.cn

[D01] 创建数组 / 列表
来源：http://vb.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xl.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qw.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xr.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sx.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jr.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://aw.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://ln.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://af.9csxet.cn

[D02] 追加元素到末尾
来源：http://ga.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wv.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mo.lnxyls.cn

JS:   arr.push(4);
来源：http://tp.muxihuayi.cn

TS:   arr.push(4);
来源：http://tx.hnjuh.cn

Java: list.add(4);
来源：http://je.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://ky.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://si.newstarts.cn

C#:   list.Add(4);
来源：http://rt.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://jq.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://me.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eo.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ey.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://ls.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://jd.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ze.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://fi.lnxyls.cn

[D04] 删除元素
来源：http://vr.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uj.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fh.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xi.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://cx.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ur.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iu.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wj.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zi.yuexingan06.cn

[D05] 访问与修改元素
来源：http://hb.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kv.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yz.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sy.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://hj.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://gi.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://to.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qo.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nd.muxihuayi.cn

[D06] 数组长度
来源：http://fg.panjiajie.cn

Py:   len(arr)
来源：http://ff.yuntaijiaju.cn

PHP:  count($arr);
来源：http://nm.huanxung.cn

JS:   arr.length
来源：http://nw.9csxet.cn

TS:   arr.length
来源：http://vi.shxzukj.cn

Java: list.size();
来源：http://yq.jianghongdianzi.cn

Go:   len(arr)
来源：http://fm.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://zm.colortex.cn

C#:   list.Count;
来源：http://dq.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://mj.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://as.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://um.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://tk.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://pf.szsharing.cn

Java: list.subList(1, 4);
来源：http://yw.hnjuh.cn

Go:   arr[1:4]
来源：http://he.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://xx.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://ho.huanxung.cn

[D08] 合并两个数组
来源：http://vf.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://ww.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://hk.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://eg.asd995.cn

TS:   [...a, ...b];
来源：http://pd.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bv.asd995.cn

Go:   append(a, b...)
来源：http://yy.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://yd.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://qh.muxihuayi.cn

[D09] 排序（升序）
来源：http://va.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://mb.panjiajie.cn

PHP:  sort($arr);
来源：http://jk.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vv.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yo.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hn.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wc.asd995.cn

Ruby: arr.sort
来源：http://oe.szsharing.cn

C#:   list.Sort();
来源：http://fo.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ax.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ac.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dv.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fb.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uo.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tk.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qr.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lr.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gh.colortex.cn

[D11] 反转数组
来源：http://ym.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hr.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://mu.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zo.nszjky.cn

TS:   [...arr].reverse();
来源：http://ol.asd995.cn

Java: Collections.reverse(list);
来源：http://bq.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://yt.hnjuh.cn

Ruby: arr.reverse
来源：http://pi.yuexingan06.cn

C#:   list.Reverse();
来源：http://fk.panjiajie.cn

[D12] 查找元素下标
来源：http://lt.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://rd.newstarts.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dt.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hf.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ke.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uo.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://tw.nicolike.cn

Ruby: arr.index(x)
来源：http://nl.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://uu.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://pp.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rg.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hu.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://yf.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://ot.yuexingan06.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yw.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ho.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qz.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://iw.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://xl.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eh.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jd.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://gi.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://qq.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fp.muxihuayi.cn

Go:   // 手写循环
来源：http://ia.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dp.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rl.yuntaijiaju.cn

[D15] 去重
来源：http://wq.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://by.hnjuh.cn

PHP:  array_unique($arr);
来源：http://bn.szsharing.cn

JS:   [...new Set(arr)]
来源：http://rk.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://za.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ns.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qi.nszjky.cn

Ruby: arr.uniq
来源：http://oz.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://mi.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://xf.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ao.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hg.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hm.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dl.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bg.chemitech.net.cn

Go:   // 手写循环累加
来源：http://wn.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://be.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://zz.nicolike.cn

[D17] 最大值与最小值
来源：http://ad.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://mc.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://mi.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sh.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://pl.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kl.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ej.huixinmuqiang.cn

Ruby: arr.max;  arr.min
来源：http://jb.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://kh.asd995.cn

[D18] 扁平化嵌套数组
来源：http://zf.muxihuayi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cs.asd995.cn

PHP:  array_merge(...$nested);
来源：http://fr.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ek.huixiangedu.cn

TS:   nested.flat();
来源：http://fw.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://er.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://va.nicolike.cn

Ruby: nested.flatten
来源：http://da.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xu.haigaiapp.cn

[D19] 按字段分组
来源：http://fn.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qx.wgjwhj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://as.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hq.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://al.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zi.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://pm.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://an.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gb.asd995.cn

[D20] 统计每个元素出现次数
来源：http://uh.yuexingan06.cn

Py:   Counter(arr)
来源：http://hk.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://cf.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aw.jctech888.com.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qt.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gg.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://qn.wgjwhj.cn

Ruby: arr.tally
来源：http://lk.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ma.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://sy.bjjhwx.cn

Py:   x in arr
来源：http://no.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://aj.jctech888.com.cn

JS:   arr.includes(x)
来源：http://tl.bjjhwx.cn

TS:   arr.includes(x)
来源：http://xe.chemitech.net.cn

Java: list.contains(x)
来源：http://oo.asd995.cn


<!-- 参考信息 -->