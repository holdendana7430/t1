代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://wi.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://tl.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://io.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ir.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ri.bjjhwx.cn

TS:   arr.map(String)
来源：http://dm.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xu.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mq.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://jr.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sv.huixiangedu.cn

[C08] 闭包
来源：http://zw.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uy.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mx.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cv.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cg.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nm.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qb.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rj.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://po.jianghongdianzi.cn

[C09] 递归
来源：http://tn.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xc.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mv.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://et.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hu.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ns.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dx.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sr.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jv.szsharing.cn

[C10] 变量作用域
来源：http://wy.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lj.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hn.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sq.yuntaijiaju.cn

TS:   同 JS
来源：http://mr.nszjky.cn

Java: 方法内为块级作用域
来源：http://ev.haigaiapp.cn

Go:   花括号块级作用域
来源：http://br.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ba.bookmarksfly.cn

C#:   块级作用域
来源：http://ns.huanxung.cn

[C11] 模块导入与导出
来源：http://ka.huixinmuqiang.cn

Py:   from module import func
来源：http://af.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ow.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://iz.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ej.hnjuh.cn

Java: import java.util.List;
来源：http://ko.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rc.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://lx.jctech888.com.cn

C#:   using System.Text;
来源：http://yq.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://oo.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://pg.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://by.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://ne.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://qw.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fv.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://yx.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://cr.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mw.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://dt.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ux.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rg.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tv.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sg.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dh.asd995.cn

Go:   func add(a, b int) int
来源：http://pw.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rq.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ce.colortex.cn

[C14] 泛型函数
来源：http://ys.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pk.521024.cn

PHP:  // 无泛型
来源：http://jv.muxihuayi.cn

JS:   // 无泛型
来源：http://vl.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uv.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pi.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zr.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://bg.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nk.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://su.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ft.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://mp.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lk.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vj.muxihuayi.cn

Java: // 无解构
来源：http://yl.shxzskj.cn

Go:   // 无解构
来源：http://lb.panjiajie.cn

Ruby: a, b = pair
来源：http://du.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://fm.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://wf.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yy.521024.cn

PHP:  // 无重载
来源：http://fk.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fg.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://zt.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qx.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://gp.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://vi.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bx.yuntaijiaju.cn

================================================================================
来源：http://ch.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://vh.bjjhwx.cn

================================================================================
来源：http://xx.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://rx.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xe.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tx.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://li.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kv.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qz.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://el.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://qq.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sb.huanxung.cn

[D02] 追加元素到末尾
来源：http://tz.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ty.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ze.muxihuayi.cn

JS:   arr.push(4);
来源：http://oi.huixiangedu.cn

TS:   arr.push(4);
来源：http://ca.huixiangedu.cn

Java: list.add(4);
来源：http://ix.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://ht.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://hw.newstarts.cn

C#:   list.Add(4);
来源：http://mo.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://jr.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://pc.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rq.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cg.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://zc.yuexingan06.cn

Java: list.add(0, 0);
来源：http://wm.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ft.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://df.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://za.yuexingan06.cn

[D04] 删除元素
来源：http://gi.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jz.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ji.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yw.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://js.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fy.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zk.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tn.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hh.haigaiapp.cn

[D05] 访问与修改元素
来源：http://oz.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ea.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rl.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cz.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://ri.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://fx.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://vp.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xn.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kp.szsharing.cn

[D06] 数组长度
来源：http://gn.hahajie.cn

Py:   len(arr)
来源：http://xq.shxzukj.cn

PHP:  count($arr);
来源：http://lu.szxytkj.cn

JS:   arr.length
来源：http://ro.panjiajie.cn

TS:   arr.length
来源：http://ad.szsharing.cn

Java: list.size();
来源：http://mc.panjiajie.cn

Go:   len(arr)
来源：http://sc.huanxung.cn

Ruby: arr.length; arr.size
来源：http://pc.jianghongdianzi.cn

C#:   list.Count;
来源：http://ax.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://hv.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gk.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qw.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://wf.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://rd.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://kr.hnjuh.cn

Go:   arr[1:4]
来源：http://gq.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://ke.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://au.newstarts.cn

[D08] 合并两个数组
来源：http://cu.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://ix.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://nh.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qz.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://co.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ij.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://kw.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://ua.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://ta.huanxung.cn

[D09] 排序（升序）
来源：http://ua.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://wv.9csxet.cn

PHP:  sort($arr);
来源：http://lt.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zg.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cr.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lb.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cy.huixinmuqiang.cn

Ruby: arr.sort
来源：http://uz.huixiangedu.cn

C#:   list.Sort();
来源：http://cj.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bh.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ff.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eo.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ll.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://to.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yz.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bc.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kc.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fv.huixiangedu.cn

[D11] 反转数组
来源：http://wf.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rq.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://zx.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ui.nicolike.cn

TS:   [...arr].reverse();
来源：http://lb.lnxyls.cn

Java: Collections.reverse(list);
来源：http://ll.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://lc.bjjhwx.cn

Ruby: arr.reverse
来源：http://zg.szxytkj.cn

C#:   list.Reverse();
来源：http://bf.panjiajie.cn

[D12] 查找元素下标
来源：http://me.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://xc.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pa.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://of.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fl.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nt.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://uf.521024.cn

Ruby: arr.index(x)
来源：http://zd.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://ky.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://fs.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xu.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zs.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://ed.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://ck.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kx.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kd.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zg.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ta.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://vq.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fq.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tq.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://jd.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://cr.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ww.9csxet.cn

Go:   // 手写循环
来源：http://ev.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ro.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fl.bookmarksfly.cn

[D15] 去重
来源：http://qt.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kv.hnjuh.cn

PHP:  array_unique($arr);
来源：http://qq.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://jg.nicolike.cn

TS:   [...new Set(arr)]
来源：http://yq.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wz.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wb.9csxet.cn

Ruby: arr.uniq
来源：http://xg.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://ge.shtwfgs.cn

[D16] 求和与平均值
来源：http://ek.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vs.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wm.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qu.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hh.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jy.gzmigu.cn

Go:   // 手写循环累加
来源：http://ig.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ok.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://ij.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://ir.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://bz.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://or.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ac.panjiajie.cn

TS:   Math.max(...arr);
来源：http://ch.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ap.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ew.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://zb.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://zb.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://pd.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xz.asd995.cn

PHP:  array_merge(...$nested);
来源：http://lu.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tw.wgjwhj.cn

TS:   nested.flat();
来源：http://yb.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uj.hnjuh.cn

Go:   // 手写双层循环
来源：http://ek.muxihuayi.cn

Ruby: nested.flatten
来源：http://wv.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sv.huixiangedu.cn

[D19] 按字段分组
来源：http://re.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zn.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rw.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fy.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mz.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yy.szxytkj.cn

Go:   // 手写 map[string][]T
来源：http://id.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hk.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uu.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://ui.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://pr.nicolike.cn

PHP:  array_count_values($arr);
来源：http://do.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lg.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kr.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ya.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://iq.shxzskj.cn

Ruby: arr.tally
来源：http://oj.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pa.521024.cn

[D21] 判断是否包含某元素
来源：http://ee.wgjwhj.cn

Py:   x in arr
来源：http://et.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://al.huixiangedu.cn

JS:   arr.includes(x)
来源：http://er.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://eu.newstarts.cn

Java: list.contains(x)
来源：http://kr.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://ba.hnjuh.cn

Ruby: arr.include?(x)
来源：http://cw.lnxyls.cn

C#:   list.Contains(x)
来源：http://wh.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://ut.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uu.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ax.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://br.newstarts.cn

TS:   [...arr];
来源：http://cx.nszjky.cn

Java: new ArrayList<>(list);
来源：http://cj.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tf.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://rb.shtwfgs.cn

C#:   new List<int>(list);
来源：http://bm.asd995.cn

[D23] reduce 累积计算
来源：http://pw.lnxyls.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ec.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ay.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ar.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bk.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yk.colortex.cn

Go:   // 手写循环
来源：http://uw.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yw.shtwfgs.cn


<!-- 参考信息 -->