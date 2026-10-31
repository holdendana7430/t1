代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yn.yuexingan06.cn

TS:   arr.map(String)
来源：http://nk.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mu.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nr.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://aq.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ix.shxzukj.cn

[C08] 闭包
来源：http://ev.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wc.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ro.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sm.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ee.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wn.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jx.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qc.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pw.muxihuayi.cn

[C09] 递归
来源：http://ik.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hc.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dn.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vn.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nl.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ic.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ey.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qo.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rq.huanxung.cn

[C10] 变量作用域
来源：http://hg.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://so.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fk.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rb.yuntaijiaju.cn

TS:   同 JS
来源：http://ux.nicolike.cn

Java: 方法内为块级作用域
来源：http://vn.muxihuayi.cn

Go:   花括号块级作用域
来源：http://zz.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lf.521024.cn

C#:   块级作用域
来源：http://ar.521024.cn

[C11] 模块导入与导出
来源：http://nj.newstarts.cn

Py:   from module import func
来源：http://ix.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gb.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uv.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://my.chemitech.net.cn

Java: import java.util.List;
来源：http://ix.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://if.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://oz.bookmarksfly.cn

C#:   using System.Text;
来源：http://fh.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://ai.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://xd.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://ys.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://mi.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://mn.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hr.9csxet.cn

Go:   func() { fmt.Println("run") }()
来源：http://fu.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://vt.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xw.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://zf.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ib.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yp.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nl.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hv.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dz.9csxet.cn

Go:   func add(a, b int) int
来源：http://xy.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tf.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dn.muxihuayi.cn

[C14] 泛型函数
来源：http://qu.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ff.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://qg.hahajie.cn

JS:   // 无泛型
来源：http://nr.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hl.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ox.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ps.9csxet.cn

Ruby: # 无泛型
来源：http://np.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fe.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://ij.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://su.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://zr.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kk.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jc.shtwfgs.cn

Java: // 无解构
来源：http://rl.nicolike.cn

Go:   // 无解构
来源：http://yt.lnxyls.cn

Ruby: a, b = pair
来源：http://yf.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://dp.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://jw.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zn.colortex.cn

PHP:  // 无重载
来源：http://fv.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://di.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://zu.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yi.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://kw.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://qo.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tj.shxzukj.cn

================================================================================
来源：http://uy.colortex.cn

D. 数组 / 列表 / 集合
来源：http://aj.hahajie.cn

================================================================================
来源：http://eb.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://uv.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yg.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ke.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dz.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dr.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wf.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://fv.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://sk.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dd.nszjky.cn

[D02] 追加元素到末尾
来源：http://ts.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qi.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sb.szxytkj.cn

JS:   arr.push(4);
来源：http://cc.shxzukj.cn

TS:   arr.push(4);
来源：http://ib.haigaiapp.cn

Java: list.add(4);
来源：http://vj.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://kp.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://rx.bjjhwx.cn

C#:   list.Add(4);
来源：http://eq.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://zh.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://mb.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yb.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bl.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://fd.haigaiapp.cn

Java: list.add(0, 0);
来源：http://sb.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uv.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cz.muxihuayi.cn

C#:   list.Insert(0, 0);
来源：http://yd.9csxet.cn

[D04] 删除元素
来源：http://bw.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ig.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lb.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gg.hnjuh.cn

TS:   arr.splice(0, 1);
来源：http://nl.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tp.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tl.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ju.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iw.newstarts.cn

[D05] 访问与修改元素
来源：http://cu.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hu.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iv.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ga.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://do.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://ls.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://lo.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://re.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ai.muxihuayi.cn

[D06] 数组长度
来源：http://iz.gzmigu.cn

Py:   len(arr)
来源：http://rr.wgjwhj.cn

PHP:  count($arr);
来源：http://vd.bookmarksfly.cn

JS:   arr.length
来源：http://wj.521024.cn

TS:   arr.length
来源：http://zh.nszjky.cn

Java: list.size();
来源：http://dv.szxytkj.cn

Go:   len(arr)
来源：http://hq.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://ca.haigaiapp.cn

C#:   list.Count;
来源：http://rw.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://md.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qb.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ij.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://rl.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://lo.huixiangedu.cn

Java: list.subList(1, 4);
来源：http://zq.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://gx.shxzskj.cn

Ruby: arr[1, 3]
来源：http://nt.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://xp.9csxet.cn

[D08] 合并两个数组
来源：http://wx.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://ru.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://nr.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ds.shxzukj.cn

TS:   [...a, ...b];
来源：http://zf.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cd.huixiangedu.cn

Go:   append(a, b...)
来源：http://pp.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://ej.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://es.asd995.cn

[D09] 排序（升序）
来源：http://xd.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://mp.colortex.cn

PHP:  sort($arr);
来源：http://yi.yuntaijiaju.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bf.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fb.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ip.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mp.szsharing.cn

Ruby: arr.sort
来源：http://vf.yuexingan06.cn

C#:   list.Sort();
来源：http://rp.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bl.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://db.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rd.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ol.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zk.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fz.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dg.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fy.jianghongdianzi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jm.lnxyls.cn

[D11] 反转数组
来源：http://fo.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pw.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://ew.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://du.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://hh.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://px.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://hc.nszjky.cn

Ruby: arr.reverse
来源：http://po.gzmigu.cn

C#:   list.Reverse();
来源：http://gm.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://co.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://bz.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bw.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yz.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eo.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ul.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://fc.chemitech.net.cn

Ruby: arr.index(x)
来源：http://sc.huanxung.cn

C#:   list.IndexOf(x);
来源：http://eg.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://dg.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vc.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://de.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://mz.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://gy.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mz.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ob.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://og.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ak.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://hg.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uf.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ya.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://jq.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://rr.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ix.wgjwhj.cn

Go:   // 手写循环
来源：http://tt.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cu.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://md.shxzukj.cn

[D15] 去重
来源：http://ds.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yx.huanxung.cn

PHP:  array_unique($arr);
来源：http://hi.newstarts.cn

JS:   [...new Set(arr)]
来源：http://iz.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://ta.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xg.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cz.hahajie.cn

Ruby: arr.uniq
来源：http://wi.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://ju.chemitech.net.cn

[D16] 求和与平均值
来源：http://ng.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wz.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gi.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zo.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nk.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fg.jctech888.com.cn

Go:   // 手写循环累加
来源：http://jh.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wn.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://jl.521024.cn

[D17] 最大值与最小值
来源：http://vi.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://ht.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://oh.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ca.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://mo.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://to.gzmigu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ou.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://kv.colortex.cn

C#:   list.Max();  list.Min()
来源：http://gx.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://no.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ef.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://cb.9csxet.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cc.bjjhwx.cn

TS:   nested.flat();
来源：http://vu.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kd.9csxet.cn

Go:   // 手写双层循环
来源：http://mj.shtwfgs.cn

Ruby: nested.flatten
来源：http://mc.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dc.bjjhwx.cn

[D19] 按字段分组
来源：http://pq.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eq.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qu.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://st.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wo.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ms.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://oh.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tz.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ae.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://de.shxzskj.cn

Py:   Counter(arr)
来源：http://yu.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://mr.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bv.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xy.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://he.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://qu.huixinmuqiang.cn

Ruby: arr.tally
来源：http://np.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jx.nicolike.cn

[D21] 判断是否包含某元素
来源：http://oy.panjiajie.cn

Py:   x in arr
来源：http://bj.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://ju.newstarts.cn

JS:   arr.includes(x)
来源：http://st.szsharing.cn

TS:   arr.includes(x)
来源：http://wg.9csxet.cn

Java: list.contains(x)
来源：http://nd.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://zq.hahajie.cn

Ruby: arr.include?(x)
来源：http://dm.hahajie.cn

C#:   list.Contains(x)
来源：http://pu.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://wq.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ig.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uj.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iu.panjiajie.cn

TS:   [...arr];
来源：http://hk.asd995.cn

Java: new ArrayList<>(list);
来源：http://mv.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ld.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://sw.muxihuayi.cn

C#:   new List<int>(list);
来源：http://xf.hahajie.cn

[D23] reduce 累积计算
来源：http://rx.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ia.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jc.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vn.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gq.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://un.jianghongdianzi.cn

Go:   // 手写循环
来源：http://bi.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gv.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ed.521024.cn

[D24] 字典 / Map 基本操作
来源：http://lw.nszjky.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yd.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ze.szxytkj.cn


<!-- 参考信息 -->