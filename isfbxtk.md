代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jc.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sv.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zl.shxzskj.cn

[C09] 递归
来源：http://nx.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fa.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uh.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yj.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pu.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wp.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vp.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bb.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zq.panjiajie.cn

[C10] 变量作用域
来源：http://ew.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nm.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://il.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vo.lnxyls.cn

TS:   同 JS
来源：http://fh.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://pa.haigaiapp.cn

Go:   花括号块级作用域
来源：http://gi.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xu.asd995.cn

C#:   块级作用域
来源：http://kq.szsharing.cn

[C11] 模块导入与导出
来源：http://xr.szxytkj.cn

Py:   from module import func
来源：http://ek.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qc.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kq.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eo.yuexingan06.cn

Java: import java.util.List;
来源：http://rm.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wq.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://et.newstarts.cn

C#:   using System.Text;
来源：http://ys.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://bn.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://mu.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://mw.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://rg.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://tj.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pn.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://op.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://no.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mn.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://lu.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pm.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zl.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ra.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xo.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kw.nszjky.cn

Go:   func add(a, b int) int
来源：http://mu.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yf.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uq.muxihuayi.cn

[C14] 泛型函数
来源：http://ra.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://si.huixiangedu.cn

PHP:  // 无泛型
来源：http://gm.panjiajie.cn

JS:   // 无泛型
来源：http://gz.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gv.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uc.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://su.newstarts.cn

Ruby: # 无泛型
来源：http://ls.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lm.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://mo.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xc.9csxet.cn

PHP:  [$a, $b] = $pair;
来源：http://vz.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tk.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bq.szsharing.cn

Java: // 无解构
来源：http://hr.panjiajie.cn

Go:   // 无解构
来源：http://tm.lnxyls.cn

Ruby: a, b = pair
来源：http://eo.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://lf.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://by.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jg.9csxet.cn

PHP:  // 无重载
来源：http://eu.nszjky.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vt.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://qg.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uf.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://rd.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://ny.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qc.yuexingan06.cn

================================================================================
来源：http://sq.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://oq.shxzukj.cn

================================================================================
来源：http://ii.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://ek.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fi.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hf.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kr.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qx.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tl.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://xa.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://xm.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lp.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://sq.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qr.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aa.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://cl.gzmigu.cn

TS:   arr.push(4);
来源：http://ya.chemitech.net.cn

Java: list.add(4);
来源：http://fv.521024.cn

Go:   arr = append(arr, 4)
来源：http://nl.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://nt.panjiajie.cn

C#:   list.Add(4);
来源：http://bu.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://tc.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://oi.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rm.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pk.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ej.haigaiapp.cn

Java: list.add(0, 0);
来源：http://qh.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://iq.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pm.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://yr.hahajie.cn

[D04] 删除元素
来源：http://ju.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xx.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mh.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iu.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://fd.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://to.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://og.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ww.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zi.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://un.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uk.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dz.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cx.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://km.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://kl.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ja.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://er.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nm.gzmigu.cn

[D06] 数组长度
来源：http://uu.9csxet.cn

Py:   len(arr)
来源：http://uz.haigaiapp.cn

PHP:  count($arr);
来源：http://xl.hnjuh.cn

JS:   arr.length
来源：http://yh.shtwfgs.cn

TS:   arr.length
来源：http://lw.jianghongdianzi.cn

Java: list.size();
来源：http://nr.shtwfgs.cn

Go:   len(arr)
来源：http://pa.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://je.szxytkj.cn

C#:   list.Count;
来源：http://nh.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://ie.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ns.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ni.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://mr.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://js.nicolike.cn

Java: list.subList(1, 4);
来源：http://pb.colortex.cn

Go:   arr[1:4]
来源：http://we.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://xl.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://yr.lnxyls.cn

[D08] 合并两个数组
来源：http://yn.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://tg.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://gw.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cx.lnxyls.cn

TS:   [...a, ...b];
来源：http://of.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aw.szxytkj.cn

Go:   append(a, b...)
来源：http://vz.huanxung.cn

Ruby: a + b;  a.concat(b)
来源：http://gu.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://ur.muxihuayi.cn

[D09] 排序（升序）
来源：http://yo.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://pl.lnxyls.cn

PHP:  sort($arr);
来源：http://qu.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ns.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ws.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://eu.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vx.panjiajie.cn

Ruby: arr.sort
来源：http://bf.bjjhwx.cn

C#:   list.Sort();
来源：http://tc.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yw.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pl.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mv.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lh.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rz.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ej.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oj.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://df.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rd.huixinmuqiang.cn

[D11] 反转数组
来源：http://gb.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tb.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://lh.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zp.521024.cn

TS:   [...arr].reverse();
来源：http://ot.asd995.cn

Java: Collections.reverse(list);
来源：http://my.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://tp.9csxet.cn

Ruby: arr.reverse
来源：http://tb.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://gz.szsharing.cn

[D12] 查找元素下标
来源：http://il.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://ig.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pj.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xq.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mf.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ld.521024.cn

Go:   slices.Index(arr, x)
来源：http://pi.huanxung.cn

Ruby: arr.index(x)
来源：http://by.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://qs.muxihuayi.cn

[D13] 过滤（保留满足条件的）
来源：http://cu.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wz.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hv.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://bj.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://ir.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sl.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nq.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ji.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ky.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://mm.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vo.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fp.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://oe.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://az.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vn.yuntaijiaju.cn

Go:   // 手写循环
来源：http://wn.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uh.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wr.asd995.cn

[D15] 去重
来源：http://nt.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sf.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://cu.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://zl.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://wr.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cl.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gy.huanxung.cn

Ruby: arr.uniq
来源：http://gv.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://rk.gzmigu.cn

[D16] 求和与平均值
来源：http://zc.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ac.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ju.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zf.yuntaijiaju.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ru.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ow.huanxung.cn

Go:   // 手写循环累加
来源：http://pu.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lk.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://eq.newstarts.cn

[D17] 最大值与最小值
来源：http://cc.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://lw.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://tm.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gn.colortex.cn

TS:   Math.max(...arr);
来源：http://uj.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tk.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fe.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://xk.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://ir.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://yc.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ai.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://nq.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dl.newstarts.cn

TS:   nested.flat();
来源：http://rf.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kz.hnjuh.cn

Go:   // 手写双层循环
来源：http://zo.hahajie.cn

Ruby: nested.flatten
来源：http://gg.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ie.huixinmuqiang.cn

[D19] 按字段分组
来源：http://zu.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hj.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ah.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ed.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ga.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iu.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://xz.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yo.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xc.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://wg.wgjwhj.cn

Py:   Counter(arr)
来源：http://jg.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://uf.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fs.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://in.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://it.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://oa.nicolike.cn

Ruby: arr.tally
来源：http://eh.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ly.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://me.bjjhwx.cn

Py:   x in arr
来源：http://om.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://si.szsharing.cn

JS:   arr.includes(x)
来源：http://wj.asd995.cn

TS:   arr.includes(x)
来源：http://gj.shtwfgs.cn

Java: list.contains(x)
来源：http://vm.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://bb.colortex.cn

Ruby: arr.include?(x)
来源：http://rn.jctech888.com.cn

C#:   list.Contains(x)
来源：http://qx.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://xm.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fj.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tf.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rx.jianghongdianzi.cn

TS:   [...arr];
来源：http://yu.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://gn.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cl.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://do.szsharing.cn

C#:   new List<int>(list);
来源：http://zx.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://bn.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gv.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ks.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bk.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xg.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://iz.9csxet.cn

Go:   // 手写循环
来源：http://ry.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xk.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rg.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://ok.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ow.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gl.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ei.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rx.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cr.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ux.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bu.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ie.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://ls.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nx.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pl.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://do.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yx.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fk.asd995.cn


<!-- 参考信息 -->