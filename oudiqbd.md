代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kg.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kp.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dk.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mz.bookmarksfly.cn

[C10] 变量作用域
来源：http://gx.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ip.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jw.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sk.panjiajie.cn

TS:   同 JS
来源：http://fn.lnxyls.cn

Java: 方法内为块级作用域
来源：http://bh.jctech888.com.cn

Go:   花括号块级作用域
来源：http://ae.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ir.hnjuh.cn

C#:   块级作用域
来源：http://so.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://qr.shxzukj.cn

Py:   from module import func
来源：http://kq.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://po.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mz.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ug.panjiajie.cn

Java: import java.util.List;
来源：http://wc.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nm.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://wh.lnxyls.cn

C#:   using System.Text;
来源：http://px.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://se.asd995.cn

Py:   (lambda: print("run"))()
来源：http://cm.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://yx.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://ng.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://nl.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://db.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://ba.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://fy.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uc.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://ne.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ou.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ya.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jq.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://an.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://de.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://bm.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uq.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://if.bookmarksfly.cn

[C14] 泛型函数
来源：http://jh.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ll.szxytkj.cn

PHP:  // 无泛型
来源：http://xc.shxzukj.cn

JS:   // 无泛型
来源：http://qq.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jk.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hv.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ao.muxihuayi.cn

Ruby: # 无泛型
来源：http://zr.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bw.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://rs.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://im.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://ai.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gg.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ui.asd995.cn

Java: // 无解构
来源：http://ls.huixinmuqiang.cn

Go:   // 无解构
来源：http://iw.shxzukj.cn

Ruby: a, b = pair
来源：http://uf.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://aa.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://in.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fg.newstarts.cn

PHP:  // 无重载
来源：http://rn.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gj.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://dv.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dt.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://em.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://vl.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ii.huixiangedu.cn

================================================================================
来源：http://af.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://vo.hnjuh.cn

================================================================================
来源：http://mq.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://nn.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ce.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://we.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pz.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://oi.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wp.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://zl.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://mu.asd995.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uy.lnxyls.cn

[D02] 追加元素到末尾
来源：http://jh.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://di.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cp.huixiangedu.cn

JS:   arr.push(4);
来源：http://wo.huixiangedu.cn

TS:   arr.push(4);
来源：http://bf.newstarts.cn

Java: list.add(4);
来源：http://lr.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://xq.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://fv.shtwfgs.cn

C#:   list.Add(4);
来源：http://wc.hahajie.cn

[D03] 在指定位置插入元素
来源：http://uu.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://ei.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ka.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vb.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://om.9csxet.cn

Java: list.add(0, 0);
来源：http://qw.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hk.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mm.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://xv.haigaiapp.cn

[D04] 删除元素
来源：http://pp.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zh.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kx.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mr.asd995.cn

TS:   arr.splice(0, 1);
来源：http://li.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kz.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fu.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nx.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xt.newstarts.cn

[D05] 访问与修改元素
来源：http://ja.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cc.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fg.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dj.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://yh.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://jf.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://ou.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fj.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nw.panjiajie.cn

[D06] 数组长度
来源：http://yy.shxzukj.cn

Py:   len(arr)
来源：http://ll.haigaiapp.cn

PHP:  count($arr);
来源：http://jn.colortex.cn

JS:   arr.length
来源：http://to.lnxyls.cn

TS:   arr.length
来源：http://zu.nicolike.cn

Java: list.size();
来源：http://ui.huanxung.cn

Go:   len(arr)
来源：http://dk.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://de.shxzukj.cn

C#:   list.Count;
来源：http://rp.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://cf.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mt.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sf.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://jj.colortex.cn

TS:   arr.slice(1, 4);
来源：http://lq.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://tp.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://ve.szxytkj.cn

Ruby: arr[1, 3]
来源：http://dq.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://jx.newstarts.cn

[D08] 合并两个数组
来源：http://yr.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://wm.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://nf.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jm.shtwfgs.cn

TS:   [...a, ...b];
来源：http://nh.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xs.muxihuayi.cn

Go:   append(a, b...)
来源：http://pe.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://yb.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://hq.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://tl.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://eu.bookmarksfly.cn

PHP:  sort($arr);
来源：http://fr.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hf.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ku.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xq.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hy.shtwfgs.cn

Ruby: arr.sort
来源：http://ac.bjjhwx.cn

C#:   list.Sort();
来源：http://xj.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kn.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vx.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yz.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ye.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://em.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xe.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://is.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rz.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dt.shtwfgs.cn

[D11] 反转数组
来源：http://yw.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kd.colortex.cn

PHP:  array_reverse($arr);
来源：http://bu.shtwfgs.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iz.szxytkj.cn

TS:   [...arr].reverse();
来源：http://rg.panjiajie.cn

Java: Collections.reverse(list);
来源：http://vp.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://yk.panjiajie.cn

Ruby: arr.reverse
来源：http://oq.chemitech.net.cn

C#:   list.Reverse();
来源：http://ei.hnjuh.cn

[D12] 查找元素下标
来源：http://kk.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://if.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hn.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vy.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xr.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tz.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://nb.nszjky.cn

Ruby: arr.index(x)
来源：http://jd.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://yt.muxihuayi.cn

[D13] 过滤（保留满足条件的）
来源：http://up.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xc.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ff.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://av.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://xn.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ob.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fx.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rn.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fw.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://bp.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://aw.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ma.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://vd.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://fv.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wk.bookmarksfly.cn

Go:   // 手写循环
来源：http://vo.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fc.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pn.huanxung.cn

[D15] 去重
来源：http://wo.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xd.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://wz.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://er.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://vj.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sn.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tc.bookmarksfly.cn

Ruby: arr.uniq
来源：http://li.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://hq.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://jk.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://du.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tp.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ii.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ya.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ct.wgjwhj.cn

Go:   // 手写循环累加
来源：http://fy.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zp.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://py.chemitech.net.cn

[D17] 最大值与最小值
来源：http://ye.bjjhwx.cn

Py:   max(arr);  min(arr)
来源：http://ws.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://oj.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://az.lnxyls.cn

TS:   Math.max(...arr);
来源：http://zl.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mo.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yy.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://ij.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://ch.521024.cn

[D18] 扁平化嵌套数组
来源：http://hu.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qm.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://pa.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yx.asd995.cn

TS:   nested.flat();
来源：http://ea.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mr.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://xq.yuexingan06.cn

Ruby: nested.flatten
来源：http://vz.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yr.nicolike.cn

[D19] 按字段分组
来源：http://ad.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rh.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://le.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tr.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kk.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ur.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://al.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vs.shxzskj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://um.colortex.cn

[D20] 统计每个元素出现次数
来源：http://uv.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://sd.newstarts.cn

PHP:  array_count_values($arr);
来源：http://gp.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://re.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qy.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zj.nicolike.cn

Go:   // 手写 map[T]int
来源：http://gp.asd995.cn

Ruby: arr.tally
来源：http://jr.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lc.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://sw.gzmigu.cn

Py:   x in arr
来源：http://cm.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://tb.huixiangedu.cn

JS:   arr.includes(x)
来源：http://fg.muxihuayi.cn

TS:   arr.includes(x)
来源：http://re.gzmigu.cn

Java: list.contains(x)
来源：http://jl.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://io.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://tv.nicolike.cn

C#:   list.Contains(x)
来源：http://wz.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://nn.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wg.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nf.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ql.chemitech.net.cn

TS:   [...arr];
来源：http://pt.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://lu.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uk.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://md.shtwfgs.cn

C#:   new List<int>(list);
来源：http://ko.gzmigu.cn

[D23] reduce 累积计算
来源：http://wq.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yk.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sl.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pk.wgjwhj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ri.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qt.haigaiapp.cn

Go:   // 手写循环
来源：http://ok.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ld.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://km.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://zx.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hc.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xe.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ko.colortex.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://at.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://in.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fc.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jp.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ht.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://nu.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ky.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ll.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lj.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bf.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ne.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xw.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tl.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ny.nszjky.cn

[D26] 数组转字符串
来源：http://xp.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://nb.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://ha.jctech888.com.cn

JS:   arr.join(", ")
来源：http://gd.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://vz.yuexingan06.cn


<!-- 参考信息 -->