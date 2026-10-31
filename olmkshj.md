代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://xg.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dn.wgjwhj.cn

[C08] 闭包
来源：http://ly.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mn.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yl.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yj.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://an.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nv.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ja.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fd.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kv.lnxyls.cn

[C09] 递归
来源：http://ig.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jo.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sb.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xy.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://de.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ly.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ny.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fv.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xy.nszjky.cn

[C10] 变量作用域
来源：http://cw.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://du.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wv.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pz.yuntaijiaju.cn

TS:   同 JS
来源：http://dg.nicolike.cn

Java: 方法内为块级作用域
来源：http://ns.hahajie.cn

Go:   花括号块级作用域
来源：http://kl.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ab.newstarts.cn

C#:   块级作用域
来源：http://oy.szxytkj.cn

[C11] 模块导入与导出
来源：http://mu.huanxung.cn

Py:   from module import func
来源：http://le.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://io.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://px.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xy.yuexingan06.cn

Java: import java.util.List;
来源：http://is.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mn.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ks.panjiajie.cn

C#:   using System.Text;
来源：http://rh.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://cy.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://dv.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://ig.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://ep.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://ev.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://no.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://cs.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://kb.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ba.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://lw.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oi.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kf.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ju.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mw.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nh.nicolike.cn

Go:   func add(a, b int) int
来源：http://yk.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sk.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ar.yuntaijiaju.cn

[C14] 泛型函数
来源：http://ut.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xq.panjiajie.cn

PHP:  // 无泛型
来源：http://jr.bookmarksfly.cn

JS:   // 无泛型
来源：http://of.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ji.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ze.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qh.haigaiapp.cn

Ruby: # 无泛型
来源：http://hb.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pp.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://uf.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ns.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://sh.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xi.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jo.nszjky.cn

Java: // 无解构
来源：http://pa.wgjwhj.cn

Go:   // 无解构
来源：http://ls.jctech888.com.cn

Ruby: a, b = pair
来源：http://ts.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://qb.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://jk.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hb.panjiajie.cn

PHP:  // 无重载
来源：http://hg.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sm.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://sp.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tc.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://uv.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://jw.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rt.yuntaijiaju.cn

================================================================================
来源：http://uj.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://ha.521024.cn

================================================================================
来源：http://kq.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://mg.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oz.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nl.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://us.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jw.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ze.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://ce.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://az.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ma.newstarts.cn

[D02] 追加元素到末尾
来源：http://jw.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pa.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bb.muxihuayi.cn

JS:   arr.push(4);
来源：http://er.shxzukj.cn

TS:   arr.push(4);
来源：http://re.nicolike.cn

Java: list.add(4);
来源：http://qs.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://zl.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://ak.haigaiapp.cn

C#:   list.Add(4);
来源：http://wq.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://yq.colortex.cn

Py:   arr.insert(0, 0)
来源：http://cz.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uf.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uf.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://zx.hnjuh.cn

Java: list.add(0, 0);
来源：http://vq.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://by.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wu.colortex.cn

C#:   list.Insert(0, 0);
来源：http://jy.bjjhwx.cn

[D04] 删除元素
来源：http://mq.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xf.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sy.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mu.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://va.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ms.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zk.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sn.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xc.wgjwhj.cn

[D05] 访问与修改元素
来源：http://ar.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wk.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nb.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qw.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://qd.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://lb.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://zd.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ce.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://od.nszjky.cn

[D06] 数组长度
来源：http://fv.nicolike.cn

Py:   len(arr)
来源：http://ki.jianghongdianzi.cn

PHP:  count($arr);
来源：http://tw.jctech888.com.cn

JS:   arr.length
来源：http://an.szxytkj.cn

TS:   arr.length
来源：http://mc.lnxyls.cn

Java: list.size();
来源：http://vn.hnjuh.cn

Go:   len(arr)
来源：http://mu.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://lf.wgjwhj.cn

C#:   list.Count;
来源：http://dw.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://ic.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wi.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yo.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://zb.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://qi.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://bg.shxzukj.cn

Go:   arr[1:4]
来源：http://ud.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://ka.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://bt.shxzskj.cn

[D08] 合并两个数组
来源：http://xb.lnxyls.cn

Py:   a + b;  a.extend(b)
来源：http://mh.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://kq.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tr.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://iq.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wh.yuexingan06.cn

Go:   append(a, b...)
来源：http://ke.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://gq.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://bv.521024.cn

[D09] 排序（升序）
来源：http://lv.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://hq.szxytkj.cn

PHP:  sort($arr);
来源：http://xn.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wl.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xf.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wo.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mz.muxihuayi.cn

Ruby: arr.sort
来源：http://ms.bookmarksfly.cn

C#:   list.Sort();
来源：http://ld.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pz.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kd.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zh.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zh.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tc.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mh.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nj.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pm.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dq.panjiajie.cn

[D11] 反转数组
来源：http://us.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qv.huanxung.cn

PHP:  array_reverse($arr);
来源：http://no.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iw.nicolike.cn

TS:   [...arr].reverse();
来源：http://je.nszjky.cn

Java: Collections.reverse(list);
来源：http://qt.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://be.szxytkj.cn

Ruby: arr.reverse
来源：http://xs.lnxyls.cn

C#:   list.Reverse();
来源：http://qv.newstarts.cn

[D12] 查找元素下标
来源：http://sy.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://ke.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hh.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ih.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tq.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gn.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://gp.haigaiapp.cn

Ruby: arr.index(x)
来源：http://js.hahajie.cn

C#:   list.IndexOf(x);
来源：http://uv.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://be.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uh.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vi.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://iq.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://ii.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ro.gzmigu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kn.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qk.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bb.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://ss.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zj.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kh.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://zz.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://zm.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yd.szsharing.cn

Go:   // 手写循环
来源：http://ou.muxihuayi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yk.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kg.chemitech.net.cn

[D15] 去重
来源：http://na.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cp.shxzskj.cn

PHP:  array_unique($arr);
来源：http://zd.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://ca.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://vt.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://om.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hd.szsharing.cn

Ruby: arr.uniq
来源：http://oa.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://qo.newstarts.cn

[D16] 求和与平均值
来源：http://xz.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jg.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ob.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fg.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nd.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fq.521024.cn

Go:   // 手写循环累加
来源：http://aw.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ux.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://yk.nszjky.cn

[D17] 最大值与最小值
来源：http://yn.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://zg.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://ao.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zj.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://bm.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cm.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rt.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://xa.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://jd.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://wr.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mo.colortex.cn

PHP:  array_merge(...$nested);
来源：http://xw.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tm.huixiangedu.cn

TS:   nested.flat();
来源：http://tv.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bb.szxytkj.cn

Go:   // 手写双层循环
来源：http://gd.nicolike.cn

Ruby: nested.flatten
来源：http://yj.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hg.haigaiapp.cn

[D19] 按字段分组
来源：http://sx.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fr.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vk.jianghongdianzi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://me.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nt.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mn.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://ga.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zx.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zl.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://dc.bookmarksfly.cn

Py:   Counter(arr)
来源：http://hc.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://rb.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ww.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sz.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://da.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://iz.9csxet.cn

Ruby: arr.tally
来源：http://ur.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gl.9csxet.cn

[D21] 判断是否包含某元素
来源：http://mz.lnxyls.cn

Py:   x in arr
来源：http://ja.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://xz.newstarts.cn

JS:   arr.includes(x)
来源：http://pf.nszjky.cn

TS:   arr.includes(x)
来源：http://sl.yuntaijiaju.cn

Java: list.contains(x)
来源：http://ai.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://od.lnxyls.cn

Ruby: arr.include?(x)
来源：http://tr.haigaiapp.cn

C#:   list.Contains(x)
来源：http://yt.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://vu.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vr.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ar.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gg.huixinmuqiang.cn

TS:   [...arr];
来源：http://tl.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://fe.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xa.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://sd.jctech888.com.cn

C#:   new List<int>(list);
来源：http://pl.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://fg.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yd.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qe.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dd.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://in.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qo.gzmigu.cn

Go:   // 手写循环
来源：http://vm.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jp.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fa.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://fr.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iy.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qc.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ao.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ux.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gr.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nu.yuntaijiaju.cn


<!-- 参考信息 -->