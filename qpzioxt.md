代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://op.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://su.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://db.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dt.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bv.gzmigu.cn

TS:   arr.map(String)
来源：http://xy.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oq.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://va.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://ap.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jb.lnxyls.cn

[C08] 闭包
来源：http://fr.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nv.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jv.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://td.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ou.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ga.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oy.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ce.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pw.szxytkj.cn

[C09] 递归
来源：http://jd.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hp.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kx.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fg.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://la.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fs.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fm.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hc.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://os.shxzskj.cn

[C10] 变量作用域
来源：http://wg.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ox.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xi.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ys.szxytkj.cn

TS:   同 JS
来源：http://sn.szsharing.cn

Java: 方法内为块级作用域
来源：http://nb.gzmigu.cn

Go:   花括号块级作用域
来源：http://rx.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fl.9csxet.cn

C#:   块级作用域
来源：http://wu.9csxet.cn

[C11] 模块导入与导出
来源：http://rk.huanxung.cn

Py:   from module import func
来源：http://xk.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rb.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kv.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ob.gzmigu.cn

Java: import java.util.List;
来源：http://dc.shtwfgs.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ic.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://oz.yuntaijiaju.cn

C#:   using System.Text;
来源：http://wp.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://fg.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://fr.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://bo.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://jj.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://vt.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ao.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://ne.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://ct.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ep.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://cj.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sc.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mj.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mg.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rg.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uu.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://vq.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qm.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xm.lnxyls.cn

[C14] 泛型函数
来源：http://qn.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://li.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://ov.bookmarksfly.cn

JS:   // 无泛型
来源：http://xy.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://re.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yk.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fp.521024.cn

Ruby: # 无泛型
来源：http://yx.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://va.colortex.cn

[C15] 解构 / 展开参数
来源：http://hz.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oq.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://cz.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gl.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nr.yuntaijiaju.cn

Java: // 无解构
来源：http://dc.shtwfgs.cn

Go:   // 无解构
来源：http://tq.9csxet.cn

Ruby: a, b = pair
来源：http://xv.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://mb.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://da.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gj.huixinmuqiang.cn

PHP:  // 无重载
来源：http://kf.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ln.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://oz.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xs.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://ha.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://eb.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pm.gzmigu.cn

================================================================================
来源：http://cd.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://xa.shtwfgs.cn

================================================================================
来源：http://mz.huanxung.cn

[D01] 创建数组 / 列表
来源：http://jc.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zm.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://be.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://aa.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kn.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dl.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://nq.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://tb.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sw.szxytkj.cn

[D02] 追加元素到末尾
来源：http://ox.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cr.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://th.hahajie.cn

JS:   arr.push(4);
来源：http://jc.szsharing.cn

TS:   arr.push(4);
来源：http://ud.shtwfgs.cn

Java: list.add(4);
来源：http://cd.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://ca.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://ua.shxzukj.cn

C#:   list.Add(4);
来源：http://hc.hahajie.cn

[D03] 在指定位置插入元素
来源：http://xe.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://ph.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://td.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vd.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://yo.yuexingan06.cn

Java: list.add(0, 0);
来源：http://mk.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://aj.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qi.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://nc.jctech888.com.cn

[D04] 删除元素
来源：http://dp.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uy.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lw.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ry.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://kq.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kb.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kj.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zp.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yg.shxzukj.cn

[D05] 访问与修改元素
来源：http://lq.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wa.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ql.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://or.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://la.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://ok.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://ib.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yn.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hi.bjjhwx.cn

[D06] 数组长度
来源：http://nj.haigaiapp.cn

Py:   len(arr)
来源：http://lv.bookmarksfly.cn

PHP:  count($arr);
来源：http://sy.szxytkj.cn

JS:   arr.length
来源：http://dj.shxzukj.cn

TS:   arr.length
来源：http://cv.shxzskj.cn

Java: list.size();
来源：http://gs.lnxyls.cn

Go:   len(arr)
来源：http://je.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://oi.nszjky.cn

C#:   list.Count;
来源：http://wh.colortex.cn

[D07] 切片 / 取子数组
来源：http://xb.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yg.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://om.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://gi.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://dv.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://xn.nicolike.cn

Go:   arr[1:4]
来源：http://un.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://ul.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://zc.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://ar.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://am.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://md.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://td.colortex.cn

TS:   [...a, ...b];
来源：http://it.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dj.haigaiapp.cn

Go:   append(a, b...)
来源：http://mc.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://lj.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://ep.szsharing.cn

[D09] 排序（升序）
来源：http://kc.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://zp.shxzukj.cn

PHP:  sort($arr);
来源：http://hz.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jh.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fs.huanxung.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ar.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ol.nszjky.cn

Ruby: arr.sort
来源：http://ak.szxytkj.cn

C#:   list.Sort();
来源：http://jr.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dk.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uj.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://as.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://su.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://un.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lw.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ob.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://de.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fs.huixiangedu.cn

[D11] 反转数组
来源：http://zp.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gq.asd995.cn

PHP:  array_reverse($arr);
来源：http://lb.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nd.asd995.cn

TS:   [...arr].reverse();
来源：http://by.newstarts.cn

Java: Collections.reverse(list);
来源：http://zc.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://dc.lnxyls.cn

Ruby: arr.reverse
来源：http://jj.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://yv.colortex.cn

[D12] 查找元素下标
来源：http://tk.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://fy.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vv.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gq.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qv.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zh.521024.cn

Go:   slices.Index(arr, x)
来源：http://fx.nszjky.cn

Ruby: arr.index(x)
来源：http://pp.huanxung.cn

C#:   list.IndexOf(x);
来源：http://dj.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://zv.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lb.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dh.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://sp.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://at.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fu.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rc.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ib.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qg.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://cg.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ai.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://en.521024.cn

JS:   arr.map(x => x * 2)
来源：http://zm.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://gi.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yh.newstarts.cn

Go:   // 手写循环
来源：http://jy.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ak.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pp.lnxyls.cn

[D15] 去重
来源：http://qd.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sf.hahajie.cn

PHP:  array_unique($arr);
来源：http://qr.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://qz.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://jc.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ll.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cu.muxihuayi.cn

Ruby: arr.uniq
来源：http://qn.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://iu.wgjwhj.cn

[D16] 求和与平均值
来源：http://zs.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ox.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pe.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sh.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ci.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yi.chemitech.net.cn

Go:   // 手写循环累加
来源：http://qq.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ew.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://kk.521024.cn

[D17] 最大值与最小值
来源：http://yo.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://rj.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://yi.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fq.hahajie.cn

TS:   Math.max(...arr);
来源：http://dn.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hh.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yt.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://kx.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://vy.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://bk.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kj.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://jc.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ue.haigaiapp.cn

TS:   nested.flat();
来源：http://zb.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jc.lnxyls.cn

Go:   // 手写双层循环
来源：http://fz.huanxung.cn

Ruby: nested.flatten
来源：http://ou.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jr.nicolike.cn

[D19] 按字段分组
来源：http://mv.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uu.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xs.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lu.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kr.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jh.asd995.cn

Go:   // 手写 map[string][]T
来源：http://ok.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zj.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://md.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://ur.nicolike.cn

Py:   Counter(arr)
来源：http://of.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://bd.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ku.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nd.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ph.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://kk.gzmigu.cn

Ruby: arr.tally
来源：http://la.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cz.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://mb.huanxung.cn

Py:   x in arr
来源：http://fb.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://jb.gzmigu.cn

JS:   arr.includes(x)
来源：http://wc.hahajie.cn

TS:   arr.includes(x)
来源：http://ax.haigaiapp.cn

Java: list.contains(x)
来源：http://vn.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://si.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://bg.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://kg.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://ic.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yk.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fk.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qj.jctech888.com.cn

TS:   [...arr];
来源：http://qa.huanxung.cn

Java: new ArrayList<>(list);
来源：http://xy.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://km.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://rb.muxihuayi.cn

C#:   new List<int>(list);
来源：http://bm.lnxyls.cn

[D23] reduce 累积计算
来源：http://aq.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ge.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ki.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yk.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kh.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://es.shxzukj.cn

Go:   // 手写循环
来源：http://sp.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hv.asd995.cn


<!-- 参考信息 -->