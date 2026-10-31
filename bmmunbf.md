代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://pg.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ah.huixiangedu.cn

[C08] 闭包
来源：http://lu.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pa.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ip.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cv.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gr.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vk.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yh.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ne.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mk.nszjky.cn

[C09] 递归
来源：http://gf.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ux.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://an.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ek.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://va.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://us.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hp.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mm.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://to.521024.cn

[C10] 变量作用域
来源：http://pi.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pz.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gm.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vm.nszjky.cn

TS:   同 JS
来源：http://mb.panjiajie.cn

Java: 方法内为块级作用域
来源：http://ay.huixiangedu.cn

Go:   花括号块级作用域
来源：http://wd.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ve.gzmigu.cn

C#:   块级作用域
来源：http://dr.colortex.cn

[C11] 模块导入与导出
来源：http://cn.shxzukj.cn

Py:   from module import func
来源：http://ni.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dn.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fb.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ec.yuexingan06.cn

Java: import java.util.List;
来源：http://io.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jx.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://xx.lnxyls.cn

C#:   using System.Text;
来源：http://ea.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://tb.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://nx.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://sl.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://zd.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://nt.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sx.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://km.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://ym.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ur.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://yw.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tq.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://es.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wp.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ls.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ul.asd995.cn

Go:   func add(a, b int) int
来源：http://ax.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sa.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mr.gzmigu.cn

[C14] 泛型函数
来源：http://cl.asd995.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vu.panjiajie.cn

PHP:  // 无泛型
来源：http://cx.huixinmuqiang.cn

JS:   // 无泛型
来源：http://pa.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://in.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ck.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://za.jctech888.com.cn

Ruby: # 无泛型
来源：http://lf.shtwfgs.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ho.521024.cn

[C15] 解构 / 展开参数
来源：http://mz.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nj.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://ac.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://it.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ay.hnjuh.cn

Java: // 无解构
来源：http://ag.bjjhwx.cn

Go:   // 无解构
来源：http://mt.haigaiapp.cn

Ruby: a, b = pair
来源：http://mz.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://yx.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://et.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xy.bjjhwx.cn

PHP:  // 无重载
来源：http://ss.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pu.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://dh.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lz.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://jd.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://ug.yuexingan06.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tj.9csxet.cn

================================================================================
来源：http://fe.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://kc.jianghongdianzi.cn

================================================================================
来源：http://vc.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://an.panjiajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zc.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vm.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xm.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hi.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ux.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://kj.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://ga.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tt.huanxung.cn

[D02] 追加元素到末尾
来源：http://cf.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bb.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fg.panjiajie.cn

JS:   arr.push(4);
来源：http://lj.panjiajie.cn

TS:   arr.push(4);
来源：http://xw.jctech888.com.cn

Java: list.add(4);
来源：http://in.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://ly.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://we.bookmarksfly.cn

C#:   list.Add(4);
来源：http://qo.nszjky.cn

[D03] 在指定位置插入元素
来源：http://iw.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://tt.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yt.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yj.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://fj.szsharing.cn

Java: list.add(0, 0);
来源：http://dz.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nq.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qd.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://nd.huanxung.cn

[D04] 删除元素
来源：http://rq.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jl.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fn.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ly.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://ul.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nv.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sz.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tf.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wh.521024.cn

[D05] 访问与修改元素
来源：http://np.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ut.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ct.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bv.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://no.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://dg.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://jg.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ln.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ps.hnjuh.cn

[D06] 数组长度
来源：http://gu.haigaiapp.cn

Py:   len(arr)
来源：http://kc.shxzskj.cn

PHP:  count($arr);
来源：http://om.nszjky.cn

JS:   arr.length
来源：http://dt.huixinmuqiang.cn

TS:   arr.length
来源：http://tx.szxytkj.cn

Java: list.size();
来源：http://rj.nicolike.cn

Go:   len(arr)
来源：http://yz.szsharing.cn

Ruby: arr.length; arr.size
来源：http://py.panjiajie.cn

C#:   list.Count;
来源：http://sr.colortex.cn

[D07] 切片 / 取子数组
来源：http://nr.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ep.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sx.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://je.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://ka.szxytkj.cn

Java: list.subList(1, 4);
来源：http://mi.asd995.cn

Go:   arr[1:4]
来源：http://rx.hahajie.cn

Ruby: arr[1, 3]
来源：http://cn.521024.cn

C#:   list.GetRange(1, 3);
来源：http://bu.jctech888.com.cn

[D08] 合并两个数组
来源：http://mk.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://tc.colortex.cn

PHP:  array_merge($a, $b);
来源：http://gl.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://iz.colortex.cn

TS:   [...a, ...b];
来源：http://kj.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mk.huixiangedu.cn

Go:   append(a, b...)
来源：http://ic.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://ps.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://ms.jctech888.com.cn

[D09] 排序（升序）
来源：http://ll.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://jp.newstarts.cn

PHP:  sort($arr);
来源：http://mp.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ym.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ih.nicolike.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vj.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dy.yuntaijiaju.cn

Ruby: arr.sort
来源：http://kk.gzmigu.cn

C#:   list.Sort();
来源：http://ca.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oo.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wc.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rx.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mv.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vz.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ro.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xy.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fm.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vl.wgjwhj.cn

[D11] 反转数组
来源：http://sl.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ej.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://xz.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qu.panjiajie.cn

TS:   [...arr].reverse();
来源：http://oi.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://zo.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://bm.asd995.cn

Ruby: arr.reverse
来源：http://sk.muxihuayi.cn

C#:   list.Reverse();
来源：http://vy.hahajie.cn

[D12] 查找元素下标
来源：http://xf.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://ra.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kd.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jr.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xo.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ic.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://ma.yuexingan06.cn

Ruby: arr.index(x)
来源：http://qb.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://dv.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://np.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zy.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bb.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://zi.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://xl.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wp.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sb.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nz.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xu.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://rq.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uq.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aq.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://fk.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://bs.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rw.colortex.cn

Go:   // 手写循环
来源：http://kp.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gx.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tb.colortex.cn

[D15] 去重
来源：http://yt.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hg.nicolike.cn

PHP:  array_unique($arr);
来源：http://sy.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://li.nicolike.cn

TS:   [...new Set(arr)]
来源：http://bh.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ni.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ji.hahajie.cn

Ruby: arr.uniq
来源：http://bw.521024.cn

C#:   list.Distinct().ToList()
来源：http://dp.hnjuh.cn

[D16] 求和与平均值
来源：http://nv.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zb.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wq.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eu.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wi.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gc.9csxet.cn

Go:   // 手写循环累加
来源：http://jl.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zv.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://ej.gzmigu.cn

[D17] 最大值与最小值
来源：http://iv.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://gt.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://wn.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://en.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://yk.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ny.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gz.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://pd.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://zc.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://lp.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mk.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://kr.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uc.huixiangedu.cn

TS:   nested.flat();
来源：http://xs.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mx.shxzskj.cn

Go:   // 手写双层循环
来源：http://zb.shxzukj.cn

Ruby: nested.flatten
来源：http://gk.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pb.huanxung.cn

[D19] 按字段分组
来源：http://lu.nicolike.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ks.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://if.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://re.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zc.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://te.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://qp.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gb.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ur.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://xw.szsharing.cn

Py:   Counter(arr)
来源：http://we.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://zq.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bl.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nd.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jk.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://tf.szxytkj.cn

Ruby: arr.tally
来源：http://lf.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bk.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://cl.newstarts.cn

Py:   x in arr
来源：http://wd.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://vx.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://wn.shxzskj.cn

TS:   arr.includes(x)
来源：http://im.bjjhwx.cn

Java: list.contains(x)
来源：http://fq.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://fi.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://js.bjjhwx.cn

C#:   list.Contains(x)
来源：http://dv.shxzskj.cn

[D22] 复制数组（避免共享引用）
来源：http://nn.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zp.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eu.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ga.bookmarksfly.cn

TS:   [...arr];
来源：http://ns.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://da.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hv.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://kr.jctech888.com.cn

C#:   new List<int>(list);
来源：http://vt.yuntaijiaju.cn

[D23] reduce 累积计算
来源：http://pa.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wc.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ba.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dj.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oi.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nt.chemitech.net.cn

Go:   // 手写循环
来源：http://zy.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nj.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ab.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://hc.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mq.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wo.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rk.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gf.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mw.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sf.jctech888.com.cn


<!-- 参考信息 -->