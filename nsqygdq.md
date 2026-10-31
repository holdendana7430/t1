代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://xt.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qi.asd995.cn

[C08] 闭包
来源：http://se.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sl.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ua.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cm.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://as.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wu.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rt.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zy.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fs.bookmarksfly.cn

[C09] 递归
来源：http://nd.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kv.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eg.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sb.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pe.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hy.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ym.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ze.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bm.newstarts.cn

[C10] 变量作用域
来源：http://pw.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uz.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://no.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lk.shtwfgs.cn

TS:   同 JS
来源：http://ip.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://kj.huanxung.cn

Go:   花括号块级作用域
来源：http://da.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sj.colortex.cn

C#:   块级作用域
来源：http://vi.colortex.cn

[C11] 模块导入与导出
来源：http://ht.shtwfgs.cn

Py:   from module import func
来源：http://po.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wx.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mt.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wc.yuexingan06.cn

Java: import java.util.List;
来源：http://jo.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wp.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://et.huixinmuqiang.cn

C#:   using System.Text;
来源：http://xq.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://il.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://sz.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://jv.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://ap.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://bb.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ns.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://tn.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://vk.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bo.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://lm.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kg.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://du.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wt.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gp.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yh.lnxyls.cn

Go:   func add(a, b int) int
来源：http://au.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dk.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pw.yuntaijiaju.cn

[C14] 泛型函数
来源：http://nj.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ux.haigaiapp.cn

PHP:  // 无泛型
来源：http://pm.szxytkj.cn

JS:   // 无泛型
来源：http://zz.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zu.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://da.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ir.muxihuayi.cn

Ruby: # 无泛型
来源：http://fv.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aw.hahajie.cn

[C15] 解构 / 展开参数
来源：http://kt.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gt.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://kg.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zy.yuntaijiaju.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tg.nszjky.cn

Java: // 无解构
来源：http://xh.panjiajie.cn

Go:   // 无解构
来源：http://ao.lnxyls.cn

Ruby: a, b = pair
来源：http://gs.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://vk.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://gg.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ra.shtwfgs.cn

PHP:  // 无重载
来源：http://kj.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ni.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://cv.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wb.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://gs.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://rd.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uf.shxzukj.cn

================================================================================
来源：http://ww.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://xb.9csxet.cn

================================================================================
来源：http://wl.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://sh.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fj.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aq.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yv.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xk.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rv.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://rz.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://es.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xo.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://yz.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cx.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://td.yuexingan06.cn

JS:   arr.push(4);
来源：http://xl.521024.cn

TS:   arr.push(4);
来源：http://vk.hnjuh.cn

Java: list.add(4);
来源：http://bt.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://ai.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://bx.muxihuayi.cn

C#:   list.Add(4);
来源：http://qz.hahajie.cn

[D03] 在指定位置插入元素
来源：http://gi.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://wq.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wg.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ra.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://xr.jctech888.com.cn

Java: list.add(0, 0);
来源：http://hb.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cq.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://io.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://st.huanxung.cn

[D04] 删除元素
来源：http://pr.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vp.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uq.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://je.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://qd.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tq.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kh.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zk.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://if.hnjuh.cn

[D05] 访问与修改元素
来源：http://ft.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ag.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qr.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rw.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://cl.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://xj.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://gh.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zp.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dv.shxzukj.cn

[D06] 数组长度
来源：http://bp.jctech888.com.cn

Py:   len(arr)
来源：http://ps.nszjky.cn

PHP:  count($arr);
来源：http://eb.asd995.cn

JS:   arr.length
来源：http://kx.shxzskj.cn

TS:   arr.length
来源：http://oy.huanxung.cn

Java: list.size();
来源：http://mm.shxzukj.cn

Go:   len(arr)
来源：http://gj.huanxung.cn

Ruby: arr.length; arr.size
来源：http://ng.jctech888.com.cn

C#:   list.Count;
来源：http://hy.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://ae.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vy.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bf.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://wi.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://xo.gzmigu.cn

Java: list.subList(1, 4);
来源：http://yn.shxzskj.cn

Go:   arr[1:4]
来源：http://zm.gzmigu.cn

Ruby: arr[1, 3]
来源：http://uf.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://xs.huixiangedu.cn

[D08] 合并两个数组
来源：http://he.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://kl.colortex.cn

PHP:  array_merge($a, $b);
来源：http://dv.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nw.521024.cn

TS:   [...a, ...b];
来源：http://af.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tj.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://sf.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://yk.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://us.huanxung.cn

[D09] 排序（升序）
来源：http://ld.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://dt.gzmigu.cn

PHP:  sort($arr);
来源：http://oj.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cj.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dj.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sp.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://my.huixiangedu.cn

Ruby: arr.sort
来源：http://jg.nicolike.cn

C#:   list.Sort();
来源：http://dc.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yt.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xz.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xr.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kp.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yf.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://it.lnxyls.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jj.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ei.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ms.shxzukj.cn

[D11] 反转数组
来源：http://zk.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mj.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://pd.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ur.szxytkj.cn

TS:   [...arr].reverse();
来源：http://kc.szsharing.cn

Java: Collections.reverse(list);
来源：http://tf.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://ws.521024.cn

Ruby: arr.reverse
来源：http://pt.nicolike.cn

C#:   list.Reverse();
来源：http://nv.panjiajie.cn

[D12] 查找元素下标
来源：http://bc.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://dx.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kh.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cv.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ed.nszjky.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mo.521024.cn

Go:   slices.Index(arr, x)
来源：http://zr.wgjwhj.cn

Ruby: arr.index(x)
来源：http://en.szsharing.cn

C#:   list.IndexOf(x);
来源：http://av.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://po.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kt.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ee.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://ij.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://si.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ec.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iu.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tc.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://km.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://xy.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fo.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gh.521024.cn

JS:   arr.map(x => x * 2)
来源：http://gc.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://qs.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gt.newstarts.cn

Go:   // 手写循环
来源：http://kb.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dw.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ia.newstarts.cn

[D15] 去重
来源：http://ic.bjjhwx.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dm.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://pz.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://jz.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://hx.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mi.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zx.hnjuh.cn

Ruby: arr.uniq
来源：http://qw.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://nk.szsharing.cn

[D16] 求和与平均值
来源：http://ey.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wf.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wl.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pa.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ch.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yf.gzmigu.cn

Go:   // 手写循环累加
来源：http://nr.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://px.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://dd.hahajie.cn

[D17] 最大值与最小值
来源：http://ez.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://ed.521024.cn

PHP:  max($arr);  min($arr);
来源：http://uq.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jz.gzmigu.cn

TS:   Math.max(...arr);
来源：http://sd.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nf.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ht.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://ai.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://nk.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://xu.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nw.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://mt.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pm.newstarts.cn

TS:   nested.flat();
来源：http://vl.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zq.nicolike.cn

Go:   // 手写双层循环
来源：http://un.bookmarksfly.cn

Ruby: nested.flatten
来源：http://px.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sf.nicolike.cn

[D19] 按字段分组
来源：http://gn.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gb.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xm.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yu.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hr.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vo.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://pk.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rd.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sw.521024.cn

[D20] 统计每个元素出现次数
来源：http://oo.gzmigu.cn

Py:   Counter(arr)
来源：http://xn.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://st.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vw.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://in.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ev.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://lj.szsharing.cn

Ruby: arr.tally
来源：http://sg.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://va.asd995.cn

[D21] 判断是否包含某元素
来源：http://mu.gzmigu.cn

Py:   x in arr
来源：http://wx.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://vi.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://fd.shxzukj.cn

TS:   arr.includes(x)
来源：http://hw.muxihuayi.cn

Java: list.contains(x)
来源：http://fo.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://vk.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://wb.huanxung.cn

C#:   list.Contains(x)
来源：http://xu.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://dn.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uh.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yn.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jr.panjiajie.cn

TS:   [...arr];
来源：http://ab.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://kp.szxytkj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://my.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://nv.shxzskj.cn

C#:   new List<int>(list);
来源：http://kb.lnxyls.cn

[D23] reduce 累积计算
来源：http://er.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ed.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ke.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ni.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://my.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rg.hnjuh.cn

Go:   // 手写循环
来源：http://es.haigaiapp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dp.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://be.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://sr.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hi.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zr.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ny.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lt.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tq.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://we.bookmarksfly.cn


<!-- 参考信息 -->