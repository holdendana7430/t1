代发 wailian999

C#:   块级作用域
来源：http://tc.nicolike.cn

[C11] 模块导入与导出
来源：http://rd.huanxung.cn

Py:   from module import func
来源：http://ju.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ii.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ew.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ef.shxzskj.cn

Java: import java.util.List;
来源：http://bs.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pl.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://jq.szsharing.cn

C#:   using System.Text;
来源：http://rq.521024.cn

[C12] 立即执行函数 IIFE
来源：http://mb.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://eg.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://xg.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://qx.gzmigu.cn

TS:   (() => { console.log("run"); })();
来源：http://in.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vc.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://jk.521024.cn

Ruby: -> { puts "run" }.call
来源：http://te.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tp.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://qu.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ee.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zi.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://js.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jf.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sn.nszjky.cn

Go:   func add(a, b int) int
来源：http://fe.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ro.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jj.huanxung.cn

[C14] 泛型函数
来源：http://rj.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fe.haigaiapp.cn

PHP:  // 无泛型
来源：http://by.bookmarksfly.cn

JS:   // 无泛型
来源：http://lf.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jg.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pb.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://my.wgjwhj.cn

Ruby: # 无泛型
来源：http://vf.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://oq.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mz.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://mv.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lo.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zm.colortex.cn

Java: // 无解构
来源：http://ig.yuexingan06.cn

Go:   // 无解构
来源：http://ro.muxihuayi.cn

Ruby: a, b = pair
来源：http://nj.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://qn.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://tw.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://us.9csxet.cn

PHP:  // 无重载
来源：http://wn.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fe.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://nt.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xd.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://uc.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://ds.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ua.9csxet.cn

================================================================================
来源：http://yy.lnxyls.cn

D. 数组 / 列表 / 集合
来源：http://gc.shtwfgs.cn

================================================================================
来源：http://wp.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://qz.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xf.shtwfgs.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bm.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qn.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lg.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://me.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://pn.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://uy.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://on.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://hd.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xz.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fk.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://pm.panjiajie.cn

TS:   arr.push(4);
来源：http://xh.haigaiapp.cn

Java: list.add(4);
来源：http://qa.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://bg.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://ai.hnjuh.cn

C#:   list.Add(4);
来源：http://fn.hahajie.cn

[D03] 在指定位置插入元素
来源：http://wd.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://mc.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jb.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://td.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://pr.chemitech.net.cn

Java: list.add(0, 0);
来源：http://bz.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bh.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ux.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://aw.chemitech.net.cn

[D04] 删除元素
来源：http://sg.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wc.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://an.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qb.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://ih.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ty.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://et.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iq.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sk.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://ft.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lg.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tl.szsharing.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eb.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://zt.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://nf.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://wv.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ul.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qf.jianghongdianzi.cn

[D06] 数组长度
来源：http://zp.shtwfgs.cn

Py:   len(arr)
来源：http://ad.yuntaijiaju.cn

PHP:  count($arr);
来源：http://uo.lnxyls.cn

JS:   arr.length
来源：http://nx.chemitech.net.cn

TS:   arr.length
来源：http://js.huixiangedu.cn

Java: list.size();
来源：http://ck.szsharing.cn

Go:   len(arr)
来源：http://sz.newstarts.cn

Ruby: arr.length; arr.size
来源：http://fj.huixinmuqiang.cn

C#:   list.Count;
来源：http://ox.9csxet.cn

[D07] 切片 / 取子数组
来源：http://bd.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pj.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wi.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://be.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://mo.hnjuh.cn

Java: list.subList(1, 4);
来源：http://xl.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://uq.gzmigu.cn

Ruby: arr[1, 3]
来源：http://mn.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://ct.panjiajie.cn

[D08] 合并两个数组
来源：http://bd.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://we.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://hj.colortex.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hy.hnjuh.cn

TS:   [...a, ...b];
来源：http://kz.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ru.szxytkj.cn

Go:   append(a, b...)
来源：http://id.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://hy.wgjwhj.cn

C#:   a.Concat(b).ToList()
来源：http://ll.nicolike.cn

[D09] 排序（升序）
来源：http://qy.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://mi.colortex.cn

PHP:  sort($arr);
来源：http://oh.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ot.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kf.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bp.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xl.nicolike.cn

Ruby: arr.sort
来源：http://fw.hnjuh.cn

C#:   list.Sort();
来源：http://vb.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gx.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zh.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qd.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fu.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tm.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bl.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ep.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://by.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nu.jianghongdianzi.cn

[D11] 反转数组
来源：http://pr.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zq.nszjky.cn

PHP:  array_reverse($arr);
来源：http://ko.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qg.9csxet.cn

TS:   [...arr].reverse();
来源：http://fl.521024.cn

Java: Collections.reverse(list);
来源：http://ct.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://co.chemitech.net.cn

Ruby: arr.reverse
来源：http://og.colortex.cn

C#:   list.Reverse();
来源：http://ze.szxytkj.cn

[D12] 查找元素下标
来源：http://gr.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://ev.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lh.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pn.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ya.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lw.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://wm.521024.cn

Ruby: arr.index(x)
来源：http://ov.9csxet.cn

C#:   list.IndexOf(x);
来源：http://rc.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://og.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cb.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://er.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://lq.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://zq.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ah.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qb.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rb.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cb.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://gi.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qz.nicolike.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ef.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://ou.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://ud.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://in.yuexingan06.cn

Go:   // 手写循环
来源：http://oj.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sf.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tt.panjiajie.cn

[D15] 去重
来源：http://vo.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kh.nszjky.cn

PHP:  array_unique($arr);
来源：http://dk.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://bv.hahajie.cn

TS:   [...new Set(arr)]
来源：http://fy.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dj.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gb.nicolike.cn

Ruby: arr.uniq
来源：http://hl.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://hy.gzmigu.cn

[D16] 求和与平均值
来源：http://qc.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wa.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zt.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eg.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://au.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lu.newstarts.cn

Go:   // 手写循环累加
来源：http://ib.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ng.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://ia.shtwfgs.cn

[D17] 最大值与最小值
来源：http://ft.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://mb.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://kp.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://at.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://io.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cp.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://im.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://rz.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://uh.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://pa.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kb.asd995.cn

PHP:  array_merge(...$nested);
来源：http://pu.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nb.panjiajie.cn

TS:   nested.flat();
来源：http://pl.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zi.yuexingan06.cn

Go:   // 手写双层循环
来源：http://tf.shxzskj.cn

Ruby: nested.flatten
来源：http://dz.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fs.521024.cn

[D19] 按字段分组
来源：http://mw.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ci.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ab.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ko.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zn.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tp.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://hz.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fz.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uq.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://bl.muxihuayi.cn

Py:   Counter(arr)
来源：http://wb.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://fm.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rm.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yd.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fm.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://zr.shtwfgs.cn

Ruby: arr.tally
来源：http://sl.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fb.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://fc.jianghongdianzi.cn

Py:   x in arr
来源：http://ov.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://ed.shxzskj.cn

JS:   arr.includes(x)
来源：http://la.jctech888.com.cn

TS:   arr.includes(x)
来源：http://yq.9csxet.cn

Java: list.contains(x)
来源：http://zx.haigaiapp.cn

Go:   slices.Contains(arr, x)
来源：http://vl.lnxyls.cn

Ruby: arr.include?(x)
来源：http://iy.9csxet.cn

C#:   list.Contains(x)
来源：http://qo.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://xj.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pl.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ke.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ei.shxzskj.cn

TS:   [...arr];
来源：http://ea.hahajie.cn

Java: new ArrayList<>(list);
来源：http://mt.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qz.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://uz.muxihuayi.cn

C#:   new List<int>(list);
来源：http://wc.9csxet.cn

[D23] reduce 累积计算
来源：http://nd.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wu.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ln.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dd.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gr.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://eo.szsharing.cn

Go:   // 手写循环
来源：http://ln.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jd.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ef.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://yv.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kz.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sj.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://id.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zx.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rg.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uz.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ee.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sn.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://ks.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bw.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pn.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vc.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yg.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yl.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rt.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ua.jianghongdianzi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rc.huixiangedu.cn

[D26] 数组转字符串
来源：http://nr.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://yp.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://xo.shxzskj.cn

JS:   arr.join(", ")
来源：http://ts.szxytkj.cn

TS:   arr.join(", ")
来源：http://qm.muxihuayi.cn

Java: String.join(", ", list)
来源：http://pz.nicolike.cn

Go:   strings.Join(strs, ", ")
来源：http://qe.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://ba.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://dn.521024.cn

================================================================================
来源：http://jh.shtwfgs.cn

E. 字符串处理
来源：http://hu.colortex.cn

================================================================================
来源：http://dp.bjjhwx.cn

[E01] 拼接字符串
来源：http://qb.huanxung.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mq.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qc.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://po.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zs.lnxyls.cn


<!-- 参考信息 -->