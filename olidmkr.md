代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zu.nicolike.cn

TS:   arr.map(String)
来源：http://jm.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nq.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ic.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://ho.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://eh.chemitech.net.cn

[C08] 闭包
来源：http://gu.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dy.lnxyls.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ly.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cf.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fl.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qe.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ly.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bf.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ir.9csxet.cn

[C09] 递归
来源：http://mr.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://es.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sz.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ho.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iw.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wf.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xq.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fy.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bn.bookmarksfly.cn

[C10] 变量作用域
来源：http://mw.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fq.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cp.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yb.huanxung.cn

TS:   同 JS
来源：http://fx.9csxet.cn

Java: 方法内为块级作用域
来源：http://hx.shxzukj.cn

Go:   花括号块级作用域
来源：http://zk.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hi.hnjuh.cn

C#:   块级作用域
来源：http://hl.nicolike.cn

[C11] 模块导入与导出
来源：http://co.szxytkj.cn

Py:   from module import func
来源：http://su.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ud.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lr.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://aq.huixiangedu.cn

Java: import java.util.List;
来源：http://eb.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lv.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://kw.bookmarksfly.cn

C#:   using System.Text;
来源：http://tv.huixiangedu.cn

[C12] 立即执行函数 IIFE
来源：http://pf.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://wc.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://se.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://wv.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://yd.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vp.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://xs.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://ok.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dh.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://zg.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oi.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://md.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uu.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://um.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nu.9csxet.cn

Go:   func add(a, b int) int
来源：http://cm.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xh.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vl.9csxet.cn

[C14] 泛型函数
来源：http://bs.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wc.szsharing.cn

PHP:  // 无泛型
来源：http://ci.asd995.cn

JS:   // 无泛型
来源：http://gx.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://km.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wg.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ln.nicolike.cn

Ruby: # 无泛型
来源：http://qb.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kn.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://cg.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wz.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://yo.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://va.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gb.9csxet.cn

Java: // 无解构
来源：http://gw.bookmarksfly.cn

Go:   // 无解构
来源：http://zr.yuexingan06.cn

Ruby: a, b = pair
来源：http://aw.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://ff.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://bp.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bp.yuntaijiaju.cn

PHP:  // 无重载
来源：http://ck.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cv.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://nl.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hl.panjiajie.cn

Go:   // 无重载：用不同函数名
来源：http://xk.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://vj.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://md.bjjhwx.cn

================================================================================
来源：http://ab.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://go.hnjuh.cn

================================================================================
来源：http://sp.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://ym.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xb.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://av.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sd.szxytkj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qt.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ex.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://ap.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://gy.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://si.shxzukj.cn

[D02] 追加元素到末尾
来源：http://op.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ly.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qg.huixiangedu.cn

JS:   arr.push(4);
来源：http://dg.shtwfgs.cn

TS:   arr.push(4);
来源：http://fo.jctech888.com.cn

Java: list.add(4);
来源：http://fp.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://ye.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ir.jctech888.com.cn

C#:   list.Add(4);
来源：http://xm.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://bx.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://cn.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wd.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sj.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://xr.521024.cn

Java: list.add(0, 0);
来源：http://qw.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ww.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wi.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://oe.jctech888.com.cn

[D04] 删除元素
来源：http://hz.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kw.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xa.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hb.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://rz.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dg.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rc.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dw.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fg.9csxet.cn

[D05] 访问与修改元素
来源：http://er.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kd.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nb.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cx.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://tv.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://wf.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://eo.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wf.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cy.bookmarksfly.cn

[D06] 数组长度
来源：http://vw.wgjwhj.cn

Py:   len(arr)
来源：http://df.panjiajie.cn

PHP:  count($arr);
来源：http://zo.shtwfgs.cn

JS:   arr.length
来源：http://fo.panjiajie.cn

TS:   arr.length
来源：http://yl.nszjky.cn

Java: list.size();
来源：http://xb.wgjwhj.cn

Go:   len(arr)
来源：http://me.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://pb.wgjwhj.cn

C#:   list.Count;
来源：http://hq.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://gl.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tr.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xf.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://ga.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://jq.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://yj.nicolike.cn

Go:   arr[1:4]
来源：http://fy.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://ha.521024.cn

C#:   list.GetRange(1, 3);
来源：http://jl.panjiajie.cn

[D08] 合并两个数组
来源：http://pw.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://ay.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://ds.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lm.hahajie.cn

TS:   [...a, ...b];
来源：http://fp.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dz.haigaiapp.cn

Go:   append(a, b...)
来源：http://fj.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://gh.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://es.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://mk.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://vf.panjiajie.cn

PHP:  sort($arr);
来源：http://zz.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hn.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tr.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gn.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kb.szsharing.cn

Ruby: arr.sort
来源：http://mr.yuntaijiaju.cn

C#:   list.Sort();
来源：http://zd.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nz.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oz.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tb.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dh.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bu.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qi.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ff.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yz.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cx.szxytkj.cn

[D11] 反转数组
来源：http://tu.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ak.hahajie.cn

PHP:  array_reverse($arr);
来源：http://hq.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uv.szsharing.cn

TS:   [...arr].reverse();
来源：http://du.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://tz.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://nz.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://sx.yuexingan06.cn

C#:   list.Reverse();
来源：http://da.panjiajie.cn

[D12] 查找元素下标
来源：http://rx.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://ku.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kf.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ww.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jo.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ti.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://ly.521024.cn

Ruby: arr.index(x)
来源：http://hw.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://so.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://hs.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://by.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://af.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://go.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://pi.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nq.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sn.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://to.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sj.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://vo.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://od.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ht.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://gx.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://zc.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qd.asd995.cn

Go:   // 手写循环
来源：http://kx.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hg.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ei.shtwfgs.cn

[D15] 去重
来源：http://lu.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gw.shxzskj.cn

PHP:  array_unique($arr);
来源：http://jp.nicolike.cn

JS:   [...new Set(arr)]
来源：http://vh.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://dt.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wq.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://oi.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://hi.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://qh.9csxet.cn

[D16] 求和与平均值
来源：http://ki.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dg.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ko.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ft.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kp.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cm.shxzskj.cn

Go:   // 手写循环累加
来源：http://oy.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cf.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://qd.jctech888.com.cn

[D17] 最大值与最小值
来源：http://mm.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://rc.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://ol.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rt.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://ih.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ox.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mb.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://fv.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://dt.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://wo.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vj.colortex.cn

PHP:  array_merge(...$nested);
来源：http://sa.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zb.huixinmuqiang.cn

TS:   nested.flat();
来源：http://lk.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gd.huanxung.cn

Go:   // 手写双层循环
来源：http://ft.lnxyls.cn

Ruby: nested.flatten
来源：http://yu.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ah.huixiangedu.cn

[D19] 按字段分组
来源：http://ra.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ae.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xo.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fz.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dq.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ul.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://le.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dw.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zg.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://zq.huixiangedu.cn

Py:   Counter(arr)
来源：http://jy.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://aq.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://td.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rm.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cf.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://er.panjiajie.cn

Ruby: arr.tally
来源：http://ix.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ko.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://fc.bjjhwx.cn

Py:   x in arr
来源：http://mz.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://hn.huixiangedu.cn

JS:   arr.includes(x)
来源：http://fy.shtwfgs.cn

TS:   arr.includes(x)
来源：http://lz.gzmigu.cn

Java: list.contains(x)
来源：http://za.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://tt.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://iz.shxzukj.cn

C#:   list.Contains(x)
来源：http://sp.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://ix.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://is.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yc.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mk.yuntaijiaju.cn

TS:   [...arr];
来源：http://ge.newstarts.cn

Java: new ArrayList<>(list);
来源：http://af.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mn.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://jq.hahajie.cn

C#:   new List<int>(list);
来源：http://yr.shtwfgs.cn

[D23] reduce 累积计算
来源：http://fk.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oi.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://br.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xv.jianghongdianzi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kn.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tn.szsharing.cn

Go:   // 手写循环
来源：http://tt.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ew.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://an.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://yo.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dj.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jm.hahajie.cn


<!-- 参考信息 -->