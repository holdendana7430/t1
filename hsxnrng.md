代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ox.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zl.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eo.gzmigu.cn

[C09] 递归
来源：http://bq.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zx.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mn.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://md.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vq.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dt.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nt.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://al.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://th.bjjhwx.cn

[C10] 变量作用域
来源：http://om.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ln.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tw.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bs.asd995.cn

TS:   同 JS
来源：http://bt.huanxung.cn

Java: 方法内为块级作用域
来源：http://ue.nszjky.cn

Go:   花括号块级作用域
来源：http://ou.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ym.shtwfgs.cn

C#:   块级作用域
来源：http://lt.huixiangedu.cn

[C11] 模块导入与导出
来源：http://fo.huanxung.cn

Py:   from module import func
来源：http://fp.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zo.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ax.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qf.jianghongdianzi.cn

Java: import java.util.List;
来源：http://jk.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pl.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://nd.bjjhwx.cn

C#:   using System.Text;
来源：http://in.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://ar.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://lf.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://lr.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://dl.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://vv.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://by.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://ek.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://on.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gc.521024.cn

[C13] 类型声明 / 类型注解
来源：http://jy.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://er.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dv.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ix.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tv.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ij.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://kv.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tq.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vw.bjjhwx.cn

[C14] 泛型函数
来源：http://rr.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mv.szxytkj.cn

PHP:  // 无泛型
来源：http://ki.szxytkj.cn

JS:   // 无泛型
来源：http://id.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tl.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jw.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://he.9csxet.cn

Ruby: # 无泛型
来源：http://di.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ev.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://ef.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hh.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://ba.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wf.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yu.bookmarksfly.cn

Java: // 无解构
来源：http://zc.521024.cn

Go:   // 无解构
来源：http://mq.szxytkj.cn

Ruby: a, b = pair
来源：http://ls.huanxung.cn

C#:   var (a, b) = pair;
来源：http://ju.521024.cn

[C16] 函数 / 方法重载
来源：http://xj.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xo.chemitech.net.cn

PHP:  // 无重载
来源：http://ha.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ep.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://pq.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ao.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://gr.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://kd.yuexingan06.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jb.jianghongdianzi.cn

================================================================================
来源：http://yr.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://da.haigaiapp.cn

================================================================================
来源：http://il.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://jj.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uv.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xu.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fr.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hh.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jd.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://vk.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://lw.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://li.nicolike.cn

[D02] 追加元素到末尾
来源：http://rf.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://id.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vw.lnxyls.cn

JS:   arr.push(4);
来源：http://tv.shxzukj.cn

TS:   arr.push(4);
来源：http://dq.hnjuh.cn

Java: list.add(4);
来源：http://ch.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://up.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://zl.huixiangedu.cn

C#:   list.Add(4);
来源：http://hq.colortex.cn

[D03] 在指定位置插入元素
来源：http://rs.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://bq.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hj.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kb.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://lk.huanxung.cn

Java: list.add(0, 0);
来源：http://sp.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kn.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yx.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://xx.hnjuh.cn

[D04] 删除元素
来源：http://fe.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ib.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cd.huixinmuqiang.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://at.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://og.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bh.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gb.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zo.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qf.shtwfgs.cn

[D05] 访问与修改元素
来源：http://lw.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ub.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zf.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mo.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://es.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://jd.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://oe.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wf.hnjuh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sx.9csxet.cn

[D06] 数组长度
来源：http://aq.panjiajie.cn

Py:   len(arr)
来源：http://rs.hahajie.cn

PHP:  count($arr);
来源：http://iy.9csxet.cn

JS:   arr.length
来源：http://pb.colortex.cn

TS:   arr.length
来源：http://qc.huixinmuqiang.cn

Java: list.size();
来源：http://qp.jianghongdianzi.cn

Go:   len(arr)
来源：http://kr.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://jr.panjiajie.cn

C#:   list.Count;
来源：http://yf.hahajie.cn

[D07] 切片 / 取子数组
来源：http://sq.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ey.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pu.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://zh.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://gm.shxzskj.cn

Java: list.subList(1, 4);
来源：http://jc.bookmarksfly.cn

Go:   arr[1:4]
来源：http://hy.hnjuh.cn

Ruby: arr[1, 3]
来源：http://rs.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://np.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://jc.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://rw.521024.cn

PHP:  array_merge($a, $b);
来源：http://ag.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yv.chemitech.net.cn

TS:   [...a, ...b];
来源：http://yq.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pa.szxytkj.cn

Go:   append(a, b...)
来源：http://bw.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://ye.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://fl.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://cy.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://by.colortex.cn

PHP:  sort($arr);
来源：http://mb.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://is.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bk.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ac.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ct.colortex.cn

Ruby: arr.sort
来源：http://av.bookmarksfly.cn

C#:   list.Sort();
来源：http://jx.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qj.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uq.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jq.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gu.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xk.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mc.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://df.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ur.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kw.jctech888.com.cn

[D11] 反转数组
来源：http://mm.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ix.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://my.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gg.colortex.cn

TS:   [...arr].reverse();
来源：http://om.gzmigu.cn

Java: Collections.reverse(list);
来源：http://cj.521024.cn

Go:   slices.Reverse(arr)
来源：http://ru.bjjhwx.cn

Ruby: arr.reverse
来源：http://ka.yuexingan06.cn

C#:   list.Reverse();
来源：http://ml.gzmigu.cn

[D12] 查找元素下标
来源：http://ty.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://yw.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://du.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gi.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dh.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mm.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://gg.gzmigu.cn

Ruby: arr.index(x)
来源：http://hc.hahajie.cn

C#:   list.IndexOf(x);
来源：http://no.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://fd.panjiajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://md.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hr.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://xx.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://qa.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xp.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dx.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xz.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bu.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://uk.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oo.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ef.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://ji.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://he.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://iu.hnjuh.cn

Go:   // 手写循环
来源：http://vu.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dd.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dv.hahajie.cn

[D15] 去重
来源：http://ua.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pq.521024.cn

PHP:  array_unique($arr);
来源：http://hx.nicolike.cn

JS:   [...new Set(arr)]
来源：http://vd.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://fy.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://et.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nv.9csxet.cn

Ruby: arr.uniq
来源：http://rv.asd995.cn

C#:   list.Distinct().ToList()
来源：http://od.shxzukj.cn

[D16] 求和与平均值
来源：http://ov.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://or.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zr.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gu.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uc.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rg.hahajie.cn

Go:   // 手写循环累加
来源：http://na.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cn.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://np.nszjky.cn

[D17] 最大值与最小值
来源：http://fq.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://tc.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://vp.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bj.asd995.cn

TS:   Math.max(...arr);
来源：http://mp.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://br.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rc.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://za.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://ir.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://zd.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pv.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://nu.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vy.bookmarksfly.cn

TS:   nested.flat();
来源：http://kd.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ko.hnjuh.cn

Go:   // 手写双层循环
来源：http://ca.huixiangedu.cn

Ruby: nested.flatten
来源：http://no.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://is.chemitech.net.cn

[D19] 按字段分组
来源：http://pu.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dd.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dq.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uu.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://em.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wx.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://xc.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://aq.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dp.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://gv.muxihuayi.cn

Py:   Counter(arr)
来源：http://ea.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://mv.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nh.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vk.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ul.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://ee.gzmigu.cn

Ruby: arr.tally
来源：http://rd.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zx.colortex.cn

[D21] 判断是否包含某元素
来源：http://px.shxzukj.cn

Py:   x in arr
来源：http://cr.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://yy.nszjky.cn

JS:   arr.includes(x)
来源：http://vy.hahajie.cn

TS:   arr.includes(x)
来源：http://ab.bookmarksfly.cn

Java: list.contains(x)
来源：http://ya.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://gj.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://pe.nicolike.cn

C#:   list.Contains(x)
来源：http://fv.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://tj.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sv.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sn.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hr.gzmigu.cn

TS:   [...arr];
来源：http://ve.9csxet.cn

Java: new ArrayList<>(list);
来源：http://hq.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ba.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://st.shxzukj.cn

C#:   new List<int>(list);
来源：http://ge.shtwfgs.cn

[D23] reduce 累积计算
来源：http://hd.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ia.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xe.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ot.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://br.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qf.jianghongdianzi.cn

Go:   // 手写循环
来源：http://oe.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hb.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zu.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://kp.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hg.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uk.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wo.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bv.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mz.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qq.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wc.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ky.wgjwhj.cn

[D25] Set 集合去重与交并差
来源：http://th.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yj.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tg.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vx.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zb.shxzskj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kj.jianghongdianzi.cn


<!-- 参考信息 -->