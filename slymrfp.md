代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://jf.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nj.huixiangedu.cn

[C08] 闭包
来源：http://dl.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ph.lnxyls.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wz.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jn.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oh.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://md.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mb.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yi.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://by.huixinmuqiang.cn

[C09] 递归
来源：http://wb.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jn.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kr.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tq.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vr.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://il.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wb.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pi.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eb.lnxyls.cn

[C10] 变量作用域
来源：http://gl.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lp.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sh.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ch.bookmarksfly.cn

TS:   同 JS
来源：http://iv.colortex.cn

Java: 方法内为块级作用域
来源：http://wk.wgjwhj.cn

Go:   花括号块级作用域
来源：http://bd.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nh.wgjwhj.cn

C#:   块级作用域
来源：http://ac.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://hc.bjjhwx.cn

Py:   from module import func
来源：http://wj.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nf.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mx.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vp.yuntaijiaju.cn

Java: import java.util.List;
来源：http://zb.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ze.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://kc.muxihuayi.cn

C#:   using System.Text;
来源：http://qt.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://cz.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://nq.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://ql.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://ty.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://ks.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wo.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://wv.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://jq.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://st.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://rg.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nb.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bt.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ve.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ms.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cp.hahajie.cn

Go:   func add(a, b int) int
来源：http://hc.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ea.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://eu.newstarts.cn

[C14] 泛型函数
来源：http://bo.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ek.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://du.asd995.cn

JS:   // 无泛型
来源：http://mw.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zu.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ne.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://md.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://kg.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ae.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://ix.yuntaijiaju.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lv.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://tf.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lo.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kl.9csxet.cn

Java: // 无解构
来源：http://fo.hnjuh.cn

Go:   // 无解构
来源：http://sw.521024.cn

Ruby: a, b = pair
来源：http://rf.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://zi.asd995.cn

[C16] 函数 / 方法重载
来源：http://zl.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tl.hahajie.cn

PHP:  // 无重载
来源：http://yz.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ht.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://th.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ki.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://xs.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://vm.colortex.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mu.chemitech.net.cn

================================================================================
来源：http://ph.colortex.cn

D. 数组 / 列表 / 集合
来源：http://no.yuexingan06.cn

================================================================================
来源：http://ug.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://pc.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jn.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ap.jianghongdianzi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ib.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gm.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mp.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://zn.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://ou.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rl.hnjuh.cn

[D02] 追加元素到末尾
来源：http://ht.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hh.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zl.bjjhwx.cn

JS:   arr.push(4);
来源：http://qm.shtwfgs.cn

TS:   arr.push(4);
来源：http://bj.huanxung.cn

Java: list.add(4);
来源：http://pn.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://cs.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://wd.szxytkj.cn

C#:   list.Add(4);
来源：http://xp.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://dd.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://yq.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iw.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dl.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://jr.hnjuh.cn

Java: list.add(0, 0);
来源：http://gw.muxihuayi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://el.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yb.panjiajie.cn

C#:   list.Insert(0, 0);
来源：http://kn.hahajie.cn

[D04] 删除元素
来源：http://wq.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bv.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oi.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dz.colortex.cn

TS:   arr.splice(0, 1);
来源：http://ar.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vr.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gk.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dl.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://az.wgjwhj.cn

[D05] 访问与修改元素
来源：http://ih.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sx.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mk.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://by.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://bu.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://bd.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://uk.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://te.muxihuayi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mk.9csxet.cn

[D06] 数组长度
来源：http://nr.haigaiapp.cn

Py:   len(arr)
来源：http://jb.bjjhwx.cn

PHP:  count($arr);
来源：http://xp.wgjwhj.cn

JS:   arr.length
来源：http://my.gzmigu.cn

TS:   arr.length
来源：http://cj.jianghongdianzi.cn

Java: list.size();
来源：http://li.chemitech.net.cn

Go:   len(arr)
来源：http://on.521024.cn

Ruby: arr.length; arr.size
来源：http://oq.yuntaijiaju.cn

C#:   list.Count;
来源：http://ig.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://bq.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://px.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sd.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://dr.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://yt.nicolike.cn

Java: list.subList(1, 4);
来源：http://sn.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://kd.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://ax.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://bb.521024.cn

[D08] 合并两个数组
来源：http://zt.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://il.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://ws.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ro.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://dv.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zs.asd995.cn

Go:   append(a, b...)
来源：http://px.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://cf.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://cb.shxzskj.cn

[D09] 排序（升序）
来源：http://qq.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://zb.hnjuh.cn

PHP:  sort($arr);
来源：http://wn.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nf.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ib.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sk.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yt.szsharing.cn

Ruby: arr.sort
来源：http://tv.bjjhwx.cn

C#:   list.Sort();
来源：http://wq.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nd.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ea.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rw.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cq.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bm.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cb.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nn.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tb.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yp.yuexingan06.cn

[D11] 反转数组
来源：http://le.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xw.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://rd.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ho.szsharing.cn

TS:   [...arr].reverse();
来源：http://uy.lnxyls.cn

Java: Collections.reverse(list);
来源：http://rg.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://ve.521024.cn

Ruby: arr.reverse
来源：http://bd.huanxung.cn

C#:   list.Reverse();
来源：http://om.haigaiapp.cn

[D12] 查找元素下标
来源：http://nv.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://zk.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bc.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oz.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mu.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fq.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://kn.nszjky.cn

Ruby: arr.index(x)
来源：http://ul.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://lr.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://ef.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jc.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fq.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://rj.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://zs.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qo.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fb.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ba.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://px.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://mt.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lj.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vp.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://rg.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://dk.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://si.asd995.cn

Go:   // 手写循环
来源：http://yr.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ff.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ic.asd995.cn

[D15] 去重
来源：http://gr.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sp.9csxet.cn

PHP:  array_unique($arr);
来源：http://xt.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://ix.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://ds.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rd.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fr.gzmigu.cn

Ruby: arr.uniq
来源：http://ou.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://ty.yuexingan06.cn

[D16] 求和与平均值
来源：http://kh.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mx.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qv.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wc.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gg.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zd.9csxet.cn

Go:   // 手写循环累加
来源：http://nv.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lx.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://qc.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://zf.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://go.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://pq.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lz.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://en.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hp.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nq.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://vd.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://qz.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://my.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jw.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://lq.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cd.yuntaijiaju.cn

TS:   nested.flat();
来源：http://eu.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ss.lnxyls.cn

Go:   // 手写双层循环
来源：http://gs.haigaiapp.cn

Ruby: nested.flatten
来源：http://ub.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pm.muxihuayi.cn

[D19] 按字段分组
来源：http://il.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kq.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vl.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mn.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sz.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wj.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://sc.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ha.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ic.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://sq.szsharing.cn

Py:   Counter(arr)
来源：http://yk.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://ta.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ul.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uw.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ht.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://qt.shtwfgs.cn

Ruby: arr.tally
来源：http://ds.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jx.newstarts.cn

[D21] 判断是否包含某元素
来源：http://wt.nszjky.cn

Py:   x in arr
来源：http://pb.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://zz.colortex.cn

JS:   arr.includes(x)
来源：http://ah.gzmigu.cn

TS:   arr.includes(x)
来源：http://oq.521024.cn

Java: list.contains(x)
来源：http://nx.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://hv.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://ge.hnjuh.cn

C#:   list.Contains(x)
来源：http://vm.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://yr.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ja.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ig.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rv.nszjky.cn

TS:   [...arr];
来源：http://ni.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://ro.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fo.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://rk.wgjwhj.cn

C#:   new List<int>(list);
来源：http://pn.lnxyls.cn

[D23] reduce 累积计算
来源：http://qf.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fs.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jy.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ks.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ua.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mj.wgjwhj.cn

Go:   // 手写循环
来源：http://dr.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rf.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zr.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://hu.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://je.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yc.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ti.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tw.shxzukj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iu.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bg.colortex.cn


<!-- 参考信息 -->