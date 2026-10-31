代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://xz.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lg.haigaiapp.cn

[C08] 闭包
来源：http://sh.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kd.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lh.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dp.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kh.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ao.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://be.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yy.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fu.hnjuh.cn

[C09] 递归
来源：http://uv.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://la.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ci.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vz.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://um.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yj.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dx.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rd.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://if.gzmigu.cn

[C10] 变量作用域
来源：http://xo.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qo.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://md.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gw.lnxyls.cn

TS:   同 JS
来源：http://qt.shxzukj.cn

Java: 方法内为块级作用域
来源：http://vb.huanxung.cn

Go:   花括号块级作用域
来源：http://lh.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tt.huanxung.cn

C#:   块级作用域
来源：http://mv.yuexingan06.cn

[C11] 模块导入与导出
来源：http://eo.huixinmuqiang.cn

Py:   from module import func
来源：http://po.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://na.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tp.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zl.shxzukj.cn

Java: import java.util.List;
来源：http://ym.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://po.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://ss.haigaiapp.cn

C#:   using System.Text;
来源：http://xb.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://gx.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://zq.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://qk.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://yh.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://wc.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://et.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://zh.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://ya.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jm.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://zq.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vb.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fl.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ah.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pr.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qg.521024.cn

Go:   func add(a, b int) int
来源：http://lb.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cw.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uo.wgjwhj.cn

[C14] 泛型函数
来源：http://yo.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uk.hahajie.cn

PHP:  // 无泛型
来源：http://wy.nszjky.cn

JS:   // 无泛型
来源：http://bj.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iu.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cd.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://en.nicolike.cn

Ruby: # 无泛型
来源：http://hl.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nd.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://kz.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ez.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://os.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://de.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zk.newstarts.cn

Java: // 无解构
来源：http://qr.bookmarksfly.cn

Go:   // 无解构
来源：http://vq.shxzskj.cn

Ruby: a, b = pair
来源：http://ek.szsharing.cn

C#:   var (a, b) = pair;
来源：http://cw.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://bc.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kg.newstarts.cn

PHP:  // 无重载
来源：http://rd.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rd.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://vj.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://im.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://rc.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://jn.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xo.colortex.cn

================================================================================
来源：http://fb.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://gn.gzmigu.cn

================================================================================
来源：http://at.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://mc.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pw.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iz.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ml.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ni.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fe.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://vk.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://ow.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wl.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://xo.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vb.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tg.haigaiapp.cn

JS:   arr.push(4);
来源：http://vo.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://jx.9csxet.cn

Java: list.add(4);
来源：http://tg.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://tq.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://sz.huanxung.cn

C#:   list.Add(4);
来源：http://ko.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://qp.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://jg.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fe.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kf.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://sj.muxihuayi.cn

Java: list.add(0, 0);
来源：http://de.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ju.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vx.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://ik.jianghongdianzi.cn

[D04] 删除元素
来源：http://ms.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zp.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gr.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://so.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://mj.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qz.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vx.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ym.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tq.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://py.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yj.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nj.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fd.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://dt.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://ff.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://rj.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://un.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iu.shtwfgs.cn

[D06] 数组长度
来源：http://qz.9csxet.cn

Py:   len(arr)
来源：http://to.asd995.cn

PHP:  count($arr);
来源：http://tr.shxzukj.cn

JS:   arr.length
来源：http://og.jctech888.com.cn

TS:   arr.length
来源：http://wj.yuexingan06.cn

Java: list.size();
来源：http://di.szsharing.cn

Go:   len(arr)
来源：http://tp.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://co.szxytkj.cn

C#:   list.Count;
来源：http://af.nszjky.cn

[D07] 切片 / 取子数组
来源：http://ba.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qp.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lk.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://nw.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://um.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://ee.nszjky.cn

Go:   arr[1:4]
来源：http://es.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://tw.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://jr.chemitech.net.cn

[D08] 合并两个数组
来源：http://vt.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://mq.asd995.cn

PHP:  array_merge($a, $b);
来源：http://xr.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zk.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://db.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ge.hahajie.cn

Go:   append(a, b...)
来源：http://gv.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://jw.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://oy.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://yx.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://cr.muxihuayi.cn

PHP:  sort($arr);
来源：http://xq.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lr.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qe.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pu.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qe.yuntaijiaju.cn

Ruby: arr.sort
来源：http://wu.nicolike.cn

C#:   list.Sort();
来源：http://vc.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lw.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pj.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fg.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sf.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://at.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uf.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lb.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fo.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dn.hahajie.cn

[D11] 反转数组
来源：http://zw.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bp.nszjky.cn

PHP:  array_reverse($arr);
来源：http://lg.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zz.newstarts.cn

TS:   [...arr].reverse();
来源：http://eo.shxzskj.cn

Java: Collections.reverse(list);
来源：http://he.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://gr.bjjhwx.cn

Ruby: arr.reverse
来源：http://sa.hahajie.cn

C#:   list.Reverse();
来源：http://xn.shxzukj.cn

[D12] 查找元素下标
来源：http://ss.521024.cn

Py:   arr.index(x);  x in arr
来源：http://ef.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://na.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ay.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ux.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dz.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://bs.bjjhwx.cn

Ruby: arr.index(x)
来源：http://qv.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://mc.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://gs.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ve.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ud.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://he.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://wf.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tz.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gm.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cb.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ym.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://ge.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sy.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yj.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://ox.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://ln.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ad.yuntaijiaju.cn

Go:   // 手写循环
来源：http://xk.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bm.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sc.gzmigu.cn

[D15] 去重
来源：http://tn.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dg.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://th.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://je.nicolike.cn

TS:   [...new Set(arr)]
来源：http://dp.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tf.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jg.bookmarksfly.cn

Ruby: arr.uniq
来源：http://zq.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://aa.szxytkj.cn

[D16] 求和与平均值
来源：http://ss.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ir.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sp.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pq.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rr.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xm.yuexingan06.cn

Go:   // 手写循环累加
来源：http://tx.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ow.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://yj.jctech888.com.cn

[D17] 最大值与最小值
来源：http://ji.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://pn.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://nh.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bs.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://xi.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jg.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://op.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://io.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://pq.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://eh.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cz.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://qv.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://np.nicolike.cn

TS:   nested.flat();
来源：http://qh.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wv.bjjhwx.cn

Go:   // 手写双层循环
来源：http://kv.jctech888.com.cn

Ruby: nested.flatten
来源：http://dy.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sr.shxzskj.cn

[D19] 按字段分组
来源：http://zb.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yo.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wn.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fe.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fz.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://za.jianghongdianzi.cn

Go:   // 手写 map[string][]T
来源：http://yo.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ru.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://el.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://xe.yuexingan06.cn

Py:   Counter(arr)
来源：http://qa.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://xh.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yt.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oe.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://td.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://jn.szsharing.cn

Ruby: arr.tally
来源：http://hh.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ch.hahajie.cn

[D21] 判断是否包含某元素
来源：http://yb.asd995.cn

Py:   x in arr
来源：http://zf.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://ah.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://ko.shtwfgs.cn

TS:   arr.includes(x)
来源：http://rk.jianghongdianzi.cn

Java: list.contains(x)
来源：http://zn.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://ny.shxzskj.cn

Ruby: arr.include?(x)
来源：http://ff.bjjhwx.cn

C#:   list.Contains(x)
来源：http://cm.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://sp.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sj.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lo.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dc.gzmigu.cn

TS:   [...arr];
来源：http://bt.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://ae.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fx.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://ea.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://kz.lnxyls.cn

[D23] reduce 累积计算
来源：http://as.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wx.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wz.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uu.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tm.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fw.huixiangedu.cn

Go:   // 手写循环
来源：http://jz.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://il.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://st.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://bz.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qd.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://je.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xt.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pn.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ck.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bp.gzmigu.cn


<!-- 参考信息 -->