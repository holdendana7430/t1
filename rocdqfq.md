代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qq.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bt.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ti.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zu.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fx.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gi.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://af.nszjky.cn

[C09] 递归
来源：http://vb.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ii.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fk.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rt.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ze.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cm.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nj.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ki.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rl.yuntaijiaju.cn

[C10] 变量作用域
来源：http://zk.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tw.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qu.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oy.huixinmuqiang.cn

TS:   同 JS
来源：http://ym.shxzskj.cn

Java: 方法内为块级作用域
来源：http://le.yuexingan06.cn

Go:   花括号块级作用域
来源：http://nm.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kl.yuntaijiaju.cn

C#:   块级作用域
来源：http://rj.nicolike.cn

[C11] 模块导入与导出
来源：http://co.bjjhwx.cn

Py:   from module import func
来源：http://ko.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mi.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kl.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hk.asd995.cn

Java: import java.util.List;
来源：http://ta.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kj.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://dp.colortex.cn

C#:   using System.Text;
来源：http://dl.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://wt.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://nm.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://nv.wgjwhj.cn

JS:   (() => { console.log("run"); })();
来源：http://lj.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://ao.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oj.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://ld.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://bz.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vd.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://id.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qq.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hd.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ij.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tw.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mt.szsharing.cn

Go:   func add(a, b int) int
来源：http://sr.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rx.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kz.hahajie.cn

[C14] 泛型函数
来源：http://mw.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xl.huixiangedu.cn

PHP:  // 无泛型
来源：http://tl.huanxung.cn

JS:   // 无泛型
来源：http://qb.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ns.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eh.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://up.lnxyls.cn

Ruby: # 无泛型
来源：http://ou.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mb.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://rv.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tl.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://qo.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ho.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uq.jctech888.com.cn

Java: // 无解构
来源：http://jc.nicolike.cn

Go:   // 无解构
来源：http://gj.haigaiapp.cn

Ruby: a, b = pair
来源：http://xi.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://pc.colortex.cn

[C16] 函数 / 方法重载
来源：http://ji.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tb.huixiangedu.cn

PHP:  // 无重载
来源：http://vt.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qf.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://kl.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uh.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://ps.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://xv.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qu.colortex.cn

================================================================================
来源：http://dx.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://py.lnxyls.cn

================================================================================
来源：http://rn.huanxung.cn

[D01] 创建数组 / 列表
来源：http://ze.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kx.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xb.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://en.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bc.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zg.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://ya.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://aw.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zp.asd995.cn

[D02] 追加元素到末尾
来源：http://xy.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cw.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mc.nszjky.cn

JS:   arr.push(4);
来源：http://yn.szxytkj.cn

TS:   arr.push(4);
来源：http://uu.nszjky.cn

Java: list.add(4);
来源：http://gy.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://at.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://ah.yuexingan06.cn

C#:   list.Add(4);
来源：http://wj.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://va.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://px.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qo.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rc.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://of.asd995.cn

Java: list.add(0, 0);
来源：http://kv.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bg.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kf.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://hg.jctech888.com.cn

[D04] 删除元素
来源：http://mw.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oc.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gp.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ee.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://ze.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://do.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://us.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ag.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qy.wgjwhj.cn

[D05] 访问与修改元素
来源：http://dx.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ip.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ef.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mb.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://so.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://fc.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://ee.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hc.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nc.jianghongdianzi.cn

[D06] 数组长度
来源：http://lr.yuexingan06.cn

Py:   len(arr)
来源：http://xg.9csxet.cn

PHP:  count($arr);
来源：http://pv.hnjuh.cn

JS:   arr.length
来源：http://mu.shxzskj.cn

TS:   arr.length
来源：http://xj.gzmigu.cn

Java: list.size();
来源：http://cs.muxihuayi.cn

Go:   len(arr)
来源：http://pm.9csxet.cn

Ruby: arr.length; arr.size
来源：http://im.yuexingan06.cn

C#:   list.Count;
来源：http://fx.huanxung.cn

[D07] 切片 / 取子数组
来源：http://zp.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hm.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://le.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://xo.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://zp.newstarts.cn

Java: list.subList(1, 4);
来源：http://ib.bjjhwx.cn

Go:   arr[1:4]
来源：http://lv.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://zh.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://hw.hnjuh.cn

[D08] 合并两个数组
来源：http://pp.521024.cn

Py:   a + b;  a.extend(b)
来源：http://xa.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://ko.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ax.jctech888.com.cn

TS:   [...a, ...b];
来源：http://vb.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rn.huanxung.cn

Go:   append(a, b...)
来源：http://yv.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://ia.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://ky.huixiangedu.cn

[D09] 排序（升序）
来源：http://gw.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://hx.jctech888.com.cn

PHP:  sort($arr);
来源：http://zc.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vr.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://go.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ec.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zm.szxytkj.cn

Ruby: arr.sort
来源：http://aa.jianghongdianzi.cn

C#:   list.Sort();
来源：http://ul.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zx.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pj.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vb.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ib.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://db.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wu.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dl.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hq.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://no.jianghongdianzi.cn

[D11] 反转数组
来源：http://pp.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oi.nszjky.cn

PHP:  array_reverse($arr);
来源：http://kr.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vs.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://ca.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://wr.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://wo.bjjhwx.cn

Ruby: arr.reverse
来源：http://gr.hahajie.cn

C#:   list.Reverse();
来源：http://eg.muxihuayi.cn

[D12] 查找元素下标
来源：http://hg.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://be.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sb.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gw.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zc.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oo.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://nj.bjjhwx.cn

Ruby: arr.index(x)
来源：http://uu.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://ft.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://lu.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ay.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nr.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://in.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://wf.yuexingan06.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eo.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gc.nszjky.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dt.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vx.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://iz.haigaiapp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pi.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qj.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://wi.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://mr.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ln.yuexingan06.cn

Go:   // 手写循环
来源：http://hh.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ze.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vv.hnjuh.cn

[D15] 去重
来源：http://aj.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mb.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://cx.nszjky.cn

JS:   [...new Set(arr)]
来源：http://op.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://ad.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://au.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ug.521024.cn

Ruby: arr.uniq
来源：http://au.colortex.cn

C#:   list.Distinct().ToList()
来源：http://tt.szsharing.cn

[D16] 求和与平均值
来源：http://wc.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lr.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hl.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mz.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cd.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mx.hnjuh.cn

Go:   // 手写循环累加
来源：http://wu.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xj.jctech888.com.cn

C#:   list.Sum();  list.Average()
来源：http://fk.lnxyls.cn

[D17] 最大值与最小值
来源：http://ur.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://jx.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://dt.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ps.lnxyls.cn

TS:   Math.max(...arr);
来源：http://jo.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://px.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zq.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://nx.521024.cn

C#:   list.Max();  list.Min()
来源：http://ny.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://hw.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bl.asd995.cn

PHP:  array_merge(...$nested);
来源：http://tz.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://es.jianghongdianzi.cn

TS:   nested.flat();
来源：http://ue.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yl.yuexingan06.cn

Go:   // 手写双层循环
来源：http://ea.wgjwhj.cn

Ruby: nested.flatten
来源：http://rv.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zf.muxihuayi.cn

[D19] 按字段分组
来源：http://nh.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sy.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yn.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vv.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pu.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fy.521024.cn

Go:   // 手写 map[string][]T
来源：http://bw.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ta.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ri.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://pw.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://bi.nicolike.cn

PHP:  array_count_values($arr);
来源：http://oa.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fp.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sl.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pl.hahajie.cn

Go:   // 手写 map[T]int
来源：http://sf.jianghongdianzi.cn

Ruby: arr.tally
来源：http://iy.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://he.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://xy.shxzukj.cn

Py:   x in arr
来源：http://qc.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://zf.shtwfgs.cn

JS:   arr.includes(x)
来源：http://cq.shxzskj.cn

TS:   arr.includes(x)
来源：http://ia.wgjwhj.cn

Java: list.contains(x)
来源：http://dg.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://hu.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://bm.521024.cn

C#:   list.Contains(x)
来源：http://vk.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://ux.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eg.hnjuh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://np.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jt.huixiangedu.cn

TS:   [...arr];
来源：http://aj.nicolike.cn

Java: new ArrayList<>(list);
来源：http://wn.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bc.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://bz.muxihuayi.cn

C#:   new List<int>(list);
来源：http://jv.muxihuayi.cn

[D23] reduce 累积计算
来源：http://tr.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sx.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jr.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://db.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eo.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pv.asd995.cn

Go:   // 手写循环
来源：http://wm.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sn.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gf.jianghongdianzi.cn

[D24] 字典 / Map 基本操作
来源：http://da.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pq.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mo.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ez.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ql.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ws.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rr.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oq.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://df.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://ra.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yh.huixiangedu.cn


<!-- 参考信息 -->