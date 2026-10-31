代发 wailian999

C#:   块级作用域
来源：http://tc.huixiangedu.cn

[C11] 模块导入与导出
来源：http://pg.shxzskj.cn

Py:   from module import func
来源：http://mu.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pu.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rg.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vm.shxzukj.cn

Java: import java.util.List;
来源：http://mb.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oe.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://lg.nszjky.cn

C#:   using System.Text;
来源：http://lm.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://hg.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://wd.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://yg.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://jq.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://ni.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ur.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://cb.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://zv.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uy.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://qg.yuntaijiaju.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vg.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wb.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vg.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qw.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zw.huanxung.cn

Go:   func add(a, b int) int
来源：http://ia.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ug.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fh.szxytkj.cn

[C14] 泛型函数
来源：http://bl.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://es.shxzukj.cn

PHP:  // 无泛型
来源：http://sa.muxihuayi.cn

JS:   // 无泛型
来源：http://rj.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mk.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rd.szxytkj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kw.shxzskj.cn

Ruby: # 无泛型
来源：http://qp.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ot.9csxet.cn

[C15] 解构 / 展开参数
来源：http://rb.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ur.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://rr.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tj.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uk.hahajie.cn

Java: // 无解构
来源：http://fn.chemitech.net.cn

Go:   // 无解构
来源：http://rw.nszjky.cn

Ruby: a, b = pair
来源：http://rj.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://fp.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://sf.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wb.yuexingan06.cn

PHP:  // 无重载
来源：http://ga.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gm.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://bf.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://du.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://rn.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://tg.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://be.wgjwhj.cn

================================================================================
来源：http://hx.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://cr.lnxyls.cn

================================================================================
来源：http://gz.hahajie.cn

[D01] 创建数组 / 列表
来源：http://ql.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://aj.huixiangedu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nz.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fv.szxytkj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nf.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kz.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://us.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://hr.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cf.szsharing.cn

[D02] 追加元素到末尾
来源：http://je.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://op.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mq.jctech888.com.cn

JS:   arr.push(4);
来源：http://ff.wgjwhj.cn

TS:   arr.push(4);
来源：http://ly.hnjuh.cn

Java: list.add(4);
来源：http://lu.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://eo.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://bv.shtwfgs.cn

C#:   list.Add(4);
来源：http://yv.9csxet.cn

[D03] 在指定位置插入元素
来源：http://qo.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://ad.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zi.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fy.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://hh.shxzukj.cn

Java: list.add(0, 0);
来源：http://xf.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ff.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tt.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://tk.nicolike.cn

[D04] 删除元素
来源：http://ix.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xh.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://go.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fj.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://fx.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mv.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yy.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ee.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lf.panjiajie.cn

[D05] 访问与修改元素
来源：http://ln.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iy.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sy.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yz.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://fh.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://cn.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://pa.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pd.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bh.colortex.cn

[D06] 数组长度
来源：http://cy.nszjky.cn

Py:   len(arr)
来源：http://ub.hahajie.cn

PHP:  count($arr);
来源：http://bp.colortex.cn

JS:   arr.length
来源：http://fd.jctech888.com.cn

TS:   arr.length
来源：http://kn.521024.cn

Java: list.size();
来源：http://tx.colortex.cn

Go:   len(arr)
来源：http://pj.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://hs.szsharing.cn

C#:   list.Count;
来源：http://fw.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://bo.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aj.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ox.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://ft.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://kz.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://qt.nszjky.cn

Go:   arr[1:4]
来源：http://xt.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://bg.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://pa.huixiangedu.cn

[D08] 合并两个数组
来源：http://df.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://yr.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://dv.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ih.hahajie.cn

TS:   [...a, ...b];
来源：http://fr.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sw.szsharing.cn

Go:   append(a, b...)
来源：http://qb.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://cy.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://ip.shtwfgs.cn

[D09] 排序（升序）
来源：http://lk.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ia.chemitech.net.cn

PHP:  sort($arr);
来源：http://qm.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rg.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yh.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://do.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://du.szxytkj.cn

Ruby: arr.sort
来源：http://lq.huanxung.cn

C#:   list.Sort();
来源：http://nr.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qz.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fw.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qx.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ph.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nn.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jn.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vr.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pf.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gy.nszjky.cn

[D11] 反转数组
来源：http://dn.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oi.colortex.cn

PHP:  array_reverse($arr);
来源：http://lx.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tv.nicolike.cn

TS:   [...arr].reverse();
来源：http://hg.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://jk.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://dv.huanxung.cn

Ruby: arr.reverse
来源：http://mu.colortex.cn

C#:   list.Reverse();
来源：http://bo.shtwfgs.cn

[D12] 查找元素下标
来源：http://ti.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://pp.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qv.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mk.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kq.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ia.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://wq.newstarts.cn

Ruby: arr.index(x)
来源：http://ao.newstarts.cn

C#:   list.IndexOf(x);
来源：http://ul.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://zk.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qa.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pf.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://dt.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://gr.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ys.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tr.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bf.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yv.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://ac.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cn.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dv.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://hp.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://sj.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uf.shxzskj.cn

Go:   // 手写循环
来源：http://ei.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xq.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hg.yuexingan06.cn

[D15] 去重
来源：http://if.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ex.szxytkj.cn

PHP:  array_unique($arr);
来源：http://ri.newstarts.cn

JS:   [...new Set(arr)]
来源：http://ot.asd995.cn

TS:   [...new Set(arr)]
来源：http://qe.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lc.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://th.nszjky.cn

Ruby: arr.uniq
来源：http://di.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://xz.lnxyls.cn

[D16] 求和与平均值
来源：http://ne.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mt.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gi.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dx.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://re.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sf.shtwfgs.cn

Go:   // 手写循环累加
来源：http://sa.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lo.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://im.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://wa.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://rt.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://mj.nszjky.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://km.shxzukj.cn

TS:   Math.max(...arr);
来源：http://bf.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://og.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gd.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://wv.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://xf.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://lz.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mu.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://xs.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fl.hahajie.cn

TS:   nested.flat();
来源：http://kq.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rn.shxzukj.cn

Go:   // 手写双层循环
来源：http://uv.colortex.cn

Ruby: nested.flatten
来源：http://zu.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ok.gzmigu.cn

[D19] 按字段分组
来源：http://mn.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oc.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fz.colortex.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://se.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yd.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://io.jianghongdianzi.cn

Go:   // 手写 map[string][]T
来源：http://fo.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ir.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://df.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://jj.panjiajie.cn

Py:   Counter(arr)
来源：http://zd.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://fz.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bj.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ky.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qr.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://io.shtwfgs.cn

Ruby: arr.tally
来源：http://vu.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sn.szsharing.cn

[D21] 判断是否包含某元素
来源：http://xw.gzmigu.cn

Py:   x in arr
来源：http://fo.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://ry.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://ba.bookmarksfly.cn

TS:   arr.includes(x)
来源：http://lo.chemitech.net.cn

Java: list.contains(x)
来源：http://do.haigaiapp.cn

Go:   slices.Contains(arr, x)
来源：http://hj.hnjuh.cn

Ruby: arr.include?(x)
来源：http://nr.szxytkj.cn

C#:   list.Contains(x)
来源：http://sc.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://fw.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nj.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ab.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ih.szsharing.cn

TS:   [...arr];
来源：http://ai.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://vq.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bw.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://tp.szxytkj.cn

C#:   new List<int>(list);
来源：http://qd.haigaiapp.cn

[D23] reduce 累积计算
来源：http://sf.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vr.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pv.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gm.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lv.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ob.bookmarksfly.cn

Go:   // 手写循环
来源：http://np.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xq.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fo.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://zr.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uz.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qr.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uf.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cl.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xk.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hr.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uf.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jo.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://ez.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kt.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mr.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ov.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ha.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ga.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pj.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pk.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hv.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://vj.asd995.cn

Py:   ", ".join(map(str, arr))
来源：http://to.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://ko.haigaiapp.cn

JS:   arr.join(", ")
来源：http://lz.colortex.cn

TS:   arr.join(", ")
来源：http://vq.chemitech.net.cn

Java: String.join(", ", list)
来源：http://ab.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://xr.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://in.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://le.gzmigu.cn

================================================================================
来源：http://ka.hnjuh.cn

E. 字符串处理
来源：http://vv.shtwfgs.cn

================================================================================
来源：http://ry.chemitech.net.cn

[E01] 拼接字符串
来源：http://wa.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fe.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ol.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vt.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://se.huixiangedu.cn


<!-- 参考信息 -->