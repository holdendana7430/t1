代发 wailian999

[C06] 匿名函数 / lambda
来源：http://fj.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://ah.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ww.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://be.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://ur.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jn.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ug.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://em.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mz.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://vs.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oe.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://if.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://an.9csxet.cn

TS:   arr.map(String)
来源：http://nj.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ln.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hf.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://pt.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wk.shxzskj.cn

[C08] 闭包
来源：http://mq.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aa.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hp.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xs.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hn.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mp.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yy.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gk.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mp.szsharing.cn

[C09] 递归
来源：http://wl.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fw.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ze.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tt.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bk.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ec.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mn.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vh.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yn.muxihuayi.cn

[C10] 变量作用域
来源：http://qw.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pq.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vo.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wd.hnjuh.cn

TS:   同 JS
来源：http://da.nszjky.cn

Java: 方法内为块级作用域
来源：http://jz.chemitech.net.cn

Go:   花括号块级作用域
来源：http://xd.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xg.szxytkj.cn

C#:   块级作用域
来源：http://mw.521024.cn

[C11] 模块导入与导出
来源：http://cd.panjiajie.cn

Py:   from module import func
来源：http://tc.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pe.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nj.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jn.shxzukj.cn

Java: import java.util.List;
来源：http://xr.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yf.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://ir.hnjuh.cn

C#:   using System.Text;
来源：http://ue.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://bu.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://dk.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://ww.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://dk.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://fa.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jg.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://pm.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://ir.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sj.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://go.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mg.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://io.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vt.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oe.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://st.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://hf.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gr.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tv.wgjwhj.cn

[C14] 泛型函数
来源：http://qf.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jl.yuexingan06.cn

PHP:  // 无泛型
来源：http://gx.colortex.cn

JS:   // 无泛型
来源：http://zh.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hs.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ob.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ot.chemitech.net.cn

Ruby: # 无泛型
来源：http://en.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ch.hahajie.cn

[C15] 解构 / 展开参数
来源：http://xx.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vb.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://ry.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gs.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mt.chemitech.net.cn

Java: // 无解构
来源：http://jw.yuntaijiaju.cn

Go:   // 无解构
来源：http://tk.huixiangedu.cn

Ruby: a, b = pair
来源：http://uv.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://uo.colortex.cn

[C16] 函数 / 方法重载
来源：http://kq.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ze.newstarts.cn

PHP:  // 无重载
来源：http://hw.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mv.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://vs.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qn.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://pe.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://uq.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://go.gzmigu.cn

================================================================================
来源：http://od.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://lj.shxzskj.cn

================================================================================
来源：http://xg.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://hb.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jj.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sa.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qg.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ol.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yo.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://mm.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://jx.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aa.panjiajie.cn

[D02] 追加元素到末尾
来源：http://gm.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xx.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lc.asd995.cn

JS:   arr.push(4);
来源：http://jg.521024.cn

TS:   arr.push(4);
来源：http://hl.chemitech.net.cn

Java: list.add(4);
来源：http://aw.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://ov.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://dy.huanxung.cn

C#:   list.Add(4);
来源：http://pi.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://vt.asd995.cn

Py:   arr.insert(0, 0)
来源：http://gk.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yj.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tp.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://sy.jctech888.com.cn

Java: list.add(0, 0);
来源：http://uo.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fk.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vv.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://tg.521024.cn

[D04] 删除元素
来源：http://jx.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fy.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ek.shxzskj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wb.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://vd.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vk.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xe.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pl.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iq.huanxung.cn

[D05] 访问与修改元素
来源：http://no.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bl.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dg.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ra.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://ni.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://rn.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://jo.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ub.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ni.szxytkj.cn

[D06] 数组长度
来源：http://sy.bjjhwx.cn

Py:   len(arr)
来源：http://jv.shxzukj.cn

PHP:  count($arr);
来源：http://lh.newstarts.cn

JS:   arr.length
来源：http://iw.lnxyls.cn

TS:   arr.length
来源：http://za.chemitech.net.cn

Java: list.size();
来源：http://gj.wgjwhj.cn

Go:   len(arr)
来源：http://of.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://qf.asd995.cn

C#:   list.Count;
来源：http://qw.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://sx.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xv.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gm.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://nn.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://zf.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://om.szsharing.cn

Go:   arr[1:4]
来源：http://ns.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://uh.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://mi.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://si.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://ux.colortex.cn

PHP:  array_merge($a, $b);
来源：http://fs.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cb.nicolike.cn

TS:   [...a, ...b];
来源：http://bc.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cy.huixiangedu.cn

Go:   append(a, b...)
来源：http://ny.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://dg.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://oc.panjiajie.cn

[D09] 排序（升序）
来源：http://cd.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://rp.newstarts.cn

PHP:  sort($arr);
来源：http://zo.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hy.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hp.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gl.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ku.haigaiapp.cn

Ruby: arr.sort
来源：http://kh.nszjky.cn

C#:   list.Sort();
来源：http://rp.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gb.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jh.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pc.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://um.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fc.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jn.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nj.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jt.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sw.521024.cn

[D11] 反转数组
来源：http://vv.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gq.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://gv.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ks.newstarts.cn

TS:   [...arr].reverse();
来源：http://jj.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://nf.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://al.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://py.shtwfgs.cn

C#:   list.Reverse();
来源：http://hn.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://qy.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://sm.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uq.nszjky.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wr.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dg.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://km.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://wa.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://tx.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://xq.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://ub.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ru.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xv.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://zl.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://pl.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ch.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bh.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zb.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xt.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://xz.nicolike.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mg.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sh.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://oe.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://lc.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qa.9csxet.cn

Go:   // 手写循环
来源：http://hk.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bn.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://va.chemitech.net.cn

[D15] 去重
来源：http://rt.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://he.gzmigu.cn

PHP:  array_unique($arr);
来源：http://vk.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://js.szsharing.cn

TS:   [...new Set(arr)]
来源：http://er.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ni.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ur.bjjhwx.cn

Ruby: arr.uniq
来源：http://mh.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://fn.szsharing.cn

[D16] 求和与平均值
来源：http://hq.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jn.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cg.nicolike.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://im.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://df.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lb.huixiangedu.cn

Go:   // 手写循环累加
来源：http://tw.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pm.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://li.gzmigu.cn

[D17] 最大值与最小值
来源：http://nk.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://on.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://hq.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ud.nszjky.cn

TS:   Math.max(...arr);
来源：http://os.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wi.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mo.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://cb.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://rm.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://dj.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dc.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://tx.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ph.hahajie.cn

TS:   nested.flat();
来源：http://sw.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cs.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://ty.521024.cn

Ruby: nested.flatten
来源：http://ge.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qm.9csxet.cn

[D19] 按字段分组
来源：http://wx.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yf.bookmarksfly.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ie.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sa.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tb.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ui.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://tz.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qy.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fs.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://mf.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://hj.9csxet.cn

PHP:  array_count_values($arr);
来源：http://hx.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vb.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://st.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xw.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://nt.gzmigu.cn

Ruby: arr.tally
来源：http://dx.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cj.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://ct.huixiangedu.cn

Py:   x in arr
来源：http://sq.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://wa.huixiangedu.cn

JS:   arr.includes(x)
来源：http://gb.colortex.cn

TS:   arr.includes(x)
来源：http://pv.panjiajie.cn

Java: list.contains(x)
来源：http://rg.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://sz.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://fy.shtwfgs.cn

C#:   list.Contains(x)
来源：http://yi.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://el.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ps.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lx.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fj.nszjky.cn

TS:   [...arr];
来源：http://yv.yuexingan06.cn

Java: new ArrayList<>(list);
来源：http://tn.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vt.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://oc.gzmigu.cn

C#:   new List<int>(list);
来源：http://jy.nicolike.cn


<!-- 参考信息 -->