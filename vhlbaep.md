代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gt.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yf.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://av.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oe.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jv.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zf.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fh.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ub.wgjwhj.cn

[C10] 变量作用域
来源：http://hy.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oe.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gf.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qn.panjiajie.cn

TS:   同 JS
来源：http://gn.szsharing.cn

Java: 方法内为块级作用域
来源：http://le.jctech888.com.cn

Go:   花括号块级作用域
来源：http://fx.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ds.bjjhwx.cn

C#:   块级作用域
来源：http://fa.hahajie.cn

[C11] 模块导入与导出
来源：http://ro.szxytkj.cn

Py:   from module import func
来源：http://jy.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sf.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://za.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pv.muxihuayi.cn

Java: import java.util.List;
来源：http://zi.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://me.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://qn.jctech888.com.cn

C#:   using System.Text;
来源：http://pg.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://cf.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://cg.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://qs.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://sy.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://nq.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://me.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://yw.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://bc.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xt.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://zo.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ls.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bh.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oc.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zm.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jw.shxzskj.cn

Go:   func add(a, b int) int
来源：http://bx.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lj.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jy.wgjwhj.cn

[C14] 泛型函数
来源：http://zc.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://df.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://uh.hnjuh.cn

JS:   // 无泛型
来源：http://vy.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vg.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zm.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aw.wgjwhj.cn

Ruby: # 无泛型
来源：http://ow.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jw.521024.cn

[C15] 解构 / 展开参数
来源：http://qq.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yv.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://sm.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://il.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gm.nicolike.cn

Java: // 无解构
来源：http://qo.asd995.cn

Go:   // 无解构
来源：http://lh.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://zx.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://xx.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://gh.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kw.huixinmuqiang.cn

PHP:  // 无重载
来源：http://ga.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nf.shtwfgs.cn

TS:   // 用联合类型或重载签名声明
来源：http://jp.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tz.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://gy.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://vp.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lv.huixiangedu.cn

================================================================================
来源：http://ep.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://mk.yuexingan06.cn

================================================================================
来源：http://uu.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://zt.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gd.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ce.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wl.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ef.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xy.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://gc.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://uq.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mt.szsharing.cn

[D02] 追加元素到末尾
来源：http://sl.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nd.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kw.shxzskj.cn

JS:   arr.push(4);
来源：http://ag.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://xg.muxihuayi.cn

Java: list.add(4);
来源：http://sa.newstarts.cn

Go:   arr = append(arr, 4)
来源：http://at.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://dt.gzmigu.cn

C#:   list.Add(4);
来源：http://pk.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://dt.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://tp.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jk.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fp.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://bp.lnxyls.cn

Java: list.add(0, 0);
来源：http://la.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xk.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mv.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://ok.shtwfgs.cn

[D04] 删除元素
来源：http://uo.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wx.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dg.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ps.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://ux.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qz.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dk.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qk.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://un.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://bq.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xl.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oy.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uw.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://nv.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://vv.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://vx.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zu.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zt.shxzskj.cn

[D06] 数组长度
来源：http://wr.shtwfgs.cn

Py:   len(arr)
来源：http://og.lnxyls.cn

PHP:  count($arr);
来源：http://tx.jctech888.com.cn

JS:   arr.length
来源：http://se.szsharing.cn

TS:   arr.length
来源：http://pw.colortex.cn

Java: list.size();
来源：http://nc.huixinmuqiang.cn

Go:   len(arr)
来源：http://kz.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://zg.bookmarksfly.cn

C#:   list.Count;
来源：http://ar.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://tw.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ub.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cl.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://qz.521024.cn

TS:   arr.slice(1, 4);
来源：http://yh.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://fy.panjiajie.cn

Go:   arr[1:4]
来源：http://nd.colortex.cn

Ruby: arr[1, 3]
来源：http://rz.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://no.nszjky.cn

[D08] 合并两个数组
来源：http://qq.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://dt.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://ty.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kw.shxzukj.cn

TS:   [...a, ...b];
来源：http://gl.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yh.shtwfgs.cn

Go:   append(a, b...)
来源：http://fu.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://ff.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://ud.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://zq.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://wt.bjjhwx.cn

PHP:  sort($arr);
来源：http://ot.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://th.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cd.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vh.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dx.asd995.cn

Ruby: arr.sort
来源：http://hp.gzmigu.cn

C#:   list.Sort();
来源：http://ln.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uj.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yz.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://an.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ws.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yw.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://au.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dp.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ed.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zu.huanxung.cn

[D11] 反转数组
来源：http://tm.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gy.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://ni.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fr.szsharing.cn

TS:   [...arr].reverse();
来源：http://rc.colortex.cn

Java: Collections.reverse(list);
来源：http://gw.521024.cn

Go:   slices.Reverse(arr)
来源：http://yg.bookmarksfly.cn

Ruby: arr.reverse
来源：http://uh.bjjhwx.cn

C#:   list.Reverse();
来源：http://he.panjiajie.cn

[D12] 查找元素下标
来源：http://hn.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://rf.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uc.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://df.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jv.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zp.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://yp.colortex.cn

Ruby: arr.index(x)
来源：http://ly.521024.cn

C#:   list.IndexOf(x);
来源：http://se.huanxung.cn

[D13] 过滤（保留满足条件的）
来源：http://gg.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jw.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gv.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://cf.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://mc.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ke.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ip.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fn.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://th.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://zr.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rt.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ma.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://rl.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://xq.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mh.muxihuayi.cn

Go:   // 手写循环
来源：http://ht.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lr.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gj.shxzukj.cn

[D15] 去重
来源：http://ou.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sp.hnjuh.cn

PHP:  array_unique($arr);
来源：http://gn.szsharing.cn

JS:   [...new Set(arr)]
来源：http://nu.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://yf.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mo.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xq.chemitech.net.cn

Ruby: arr.uniq
来源：http://cd.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://dm.szsharing.cn

[D16] 求和与平均值
来源：http://au.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ex.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ra.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hf.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ti.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ot.wgjwhj.cn

Go:   // 手写循环累加
来源：http://sn.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gr.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://wo.shxzskj.cn

[D17] 最大值与最小值
来源：http://ld.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://xn.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://oz.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wu.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://bd.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://df.521024.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qw.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://ab.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://jc.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://ru.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sv.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://lv.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xw.shtwfgs.cn

TS:   nested.flat();
来源：http://ge.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rm.nicolike.cn

Go:   // 手写双层循环
来源：http://fs.asd995.cn

Ruby: nested.flatten
来源：http://wt.szsharing.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kb.asd995.cn

[D19] 按字段分组
来源：http://gf.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rl.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mk.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://et.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lu.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ti.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://xs.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qz.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://on.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://hk.shtwfgs.cn

Py:   Counter(arr)
来源：http://hm.colortex.cn

PHP:  array_count_values($arr);
来源：http://pl.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sq.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vg.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fp.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://wb.bjjhwx.cn

Ruby: arr.tally
来源：http://kw.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bh.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://uq.yuexingan06.cn

Py:   x in arr
来源：http://wc.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://vj.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://ej.hnjuh.cn

TS:   arr.includes(x)
来源：http://go.hnjuh.cn

Java: list.contains(x)
来源：http://lb.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://hp.521024.cn

Ruby: arr.include?(x)
来源：http://lg.nicolike.cn

C#:   list.Contains(x)
来源：http://wu.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://gw.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vl.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wq.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kb.yuntaijiaju.cn

TS:   [...arr];
来源：http://pi.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://ew.chemitech.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://of.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://od.muxihuayi.cn

C#:   new List<int>(list);
来源：http://tb.521024.cn

[D23] reduce 累积计算
来源：http://rb.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oo.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bs.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yr.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ye.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wv.chemitech.net.cn

Go:   // 手写循环
来源：http://vh.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hk.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bf.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://ul.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qk.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qt.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fq.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fi.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bv.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rv.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ph.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zo.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://pm.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jb.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nk.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://db.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lo.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kx.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bb.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ox.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zt.chemitech.net.cn

[D26] 数组转字符串
来源：http://hd.gzmigu.cn


<!-- 参考信息 -->