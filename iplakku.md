代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lp.shxzskj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nq.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rq.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ed.nicolike.cn

[C10] 变量作用域
来源：http://vz.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ez.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rp.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mh.nszjky.cn

TS:   同 JS
来源：http://bk.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://gt.haigaiapp.cn

Go:   花括号块级作用域
来源：http://yq.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://of.haigaiapp.cn

C#:   块级作用域
来源：http://jm.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://wy.huixinmuqiang.cn

Py:   from module import func
来源：http://by.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ji.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://an.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fj.521024.cn

Java: import java.util.List;
来源：http://fr.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ou.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://dt.lnxyls.cn

C#:   using System.Text;
来源：http://oe.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://td.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://zm.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://yz.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://ib.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://bg.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ys.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://ln.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://fj.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ta.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://ff.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dy.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mw.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://po.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rh.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qb.9csxet.cn

Go:   func add(a, b int) int
来源：http://jm.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tf.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xi.shxzskj.cn

[C14] 泛型函数
来源：http://mn.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mg.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://jg.yuexingan06.cn

JS:   // 无泛型
来源：http://jd.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qn.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ks.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cc.521024.cn

Ruby: # 无泛型
来源：http://pa.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iq.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://fs.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://re.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://rd.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://be.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ur.jctech888.com.cn

Java: // 无解构
来源：http://ze.asd995.cn

Go:   // 无解构
来源：http://fv.shxzskj.cn

Ruby: a, b = pair
来源：http://yr.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://hy.nicolike.cn

[C16] 函数 / 方法重载
来源：http://sp.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vk.huixiangedu.cn

PHP:  // 无重载
来源：http://yv.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tn.huixinmuqiang.cn

TS:   // 用联合类型或重载签名声明
来源：http://il.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://di.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://fz.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://sj.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cv.jianghongdianzi.cn

================================================================================
来源：http://qj.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://he.521024.cn

================================================================================
来源：http://el.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://oh.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vu.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vo.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://do.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ri.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xw.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://uu.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://lw.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ij.hnjuh.cn

[D02] 追加元素到末尾
来源：http://ow.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vs.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nn.szsharing.cn

JS:   arr.push(4);
来源：http://tr.chemitech.net.cn

TS:   arr.push(4);
来源：http://vv.panjiajie.cn

Java: list.add(4);
来源：http://ym.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://bb.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://vf.jctech888.com.cn

C#:   list.Add(4);
来源：http://xu.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://hq.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://bc.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sl.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yi.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://qq.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://cm.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jn.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zq.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://lv.shxzskj.cn

[D04] 删除元素
来源：http://jg.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ld.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sa.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ib.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://va.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sj.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vb.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ub.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mt.huanxung.cn

[D05] 访问与修改元素
来源：http://ot.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qu.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wl.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ow.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://fb.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://lg.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://zd.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cs.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qw.bjjhwx.cn

[D06] 数组长度
来源：http://ay.yuexingan06.cn

Py:   len(arr)
来源：http://by.hahajie.cn

PHP:  count($arr);
来源：http://bb.haigaiapp.cn

JS:   arr.length
来源：http://sv.jctech888.com.cn

TS:   arr.length
来源：http://hk.chemitech.net.cn

Java: list.size();
来源：http://db.colortex.cn

Go:   len(arr)
来源：http://xm.newstarts.cn

Ruby: arr.length; arr.size
来源：http://jb.chemitech.net.cn

C#:   list.Count;
来源：http://xi.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://vm.9csxet.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uq.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kv.colortex.cn

JS:   arr.slice(1, 4);
来源：http://gz.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://ye.szsharing.cn

Java: list.subList(1, 4);
来源：http://kq.jctech888.com.cn

Go:   arr[1:4]
来源：http://ys.nszjky.cn

Ruby: arr[1, 3]
来源：http://pz.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://qy.shxzukj.cn

[D08] 合并两个数组
来源：http://yq.lnxyls.cn

Py:   a + b;  a.extend(b)
来源：http://wk.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://tr.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jc.jctech888.com.cn

TS:   [...a, ...b];
来源：http://xp.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qg.bookmarksfly.cn

Go:   append(a, b...)
来源：http://ir.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://lt.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://vo.asd995.cn

[D09] 排序（升序）
来源：http://bl.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://as.muxihuayi.cn

PHP:  sort($arr);
来源：http://ag.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ff.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mx.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bh.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pi.shtwfgs.cn

Ruby: arr.sort
来源：http://lz.hahajie.cn

C#:   list.Sort();
来源：http://py.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hf.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ii.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://om.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kb.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qy.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mu.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jh.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://me.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oe.shxzukj.cn

[D11] 反转数组
来源：http://av.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mq.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://le.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vc.lnxyls.cn

TS:   [...arr].reverse();
来源：http://gm.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://ou.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://lw.yuexingan06.cn

Ruby: arr.reverse
来源：http://zx.hahajie.cn

C#:   list.Reverse();
来源：http://bn.huanxung.cn

[D12] 查找元素下标
来源：http://ci.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://pr.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ty.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zw.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ie.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sh.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://ao.nszjky.cn

Ruby: arr.index(x)
来源：http://mm.nicolike.cn

C#:   list.IndexOf(x);
来源：http://ep.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://dz.panjiajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ah.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://um.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://wa.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://ou.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gk.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vi.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uc.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sh.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://km.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ig.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gd.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://ea.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://la.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qn.521024.cn

Go:   // 手写循环
来源：http://eb.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://du.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ji.colortex.cn

[D15] 去重
来源：http://cj.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yx.szxytkj.cn

PHP:  array_unique($arr);
来源：http://xz.colortex.cn

JS:   [...new Set(arr)]
来源：http://hr.newstarts.cn

TS:   [...new Set(arr)]
来源：http://fa.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rg.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tt.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://qw.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://zh.shtwfgs.cn

[D16] 求和与平均值
来源：http://ys.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fp.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fj.gzmigu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ja.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xt.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fr.panjiajie.cn

Go:   // 手写循环累加
来源：http://kh.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://re.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://gs.gzmigu.cn

[D17] 最大值与最小值
来源：http://ii.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://fc.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://dc.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vf.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://mo.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hw.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mc.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://yg.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://cd.colortex.cn

[D18] 扁平化嵌套数组
来源：http://ms.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iy.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://yo.shxzskj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fh.huixiangedu.cn

TS:   nested.flat();
来源：http://ov.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nn.jctech888.com.cn

Go:   // 手写双层循环
来源：http://iy.shxzskj.cn

Ruby: nested.flatten
来源：http://dz.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://py.szsharing.cn

[D19] 按字段分组
来源：http://li.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ci.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fl.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xs.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cs.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qr.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://pg.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fp.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rs.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://aq.hahajie.cn

Py:   Counter(arr)
来源：http://pv.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://zp.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rc.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gj.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dn.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://dc.hahajie.cn

Ruby: arr.tally
来源：http://wd.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://js.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://hm.nicolike.cn

Py:   x in arr
来源：http://ve.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://ph.jctech888.com.cn

JS:   arr.includes(x)
来源：http://mk.bjjhwx.cn

TS:   arr.includes(x)
来源：http://dt.huanxung.cn

Java: list.contains(x)
来源：http://nz.haigaiapp.cn

Go:   slices.Contains(arr, x)
来源：http://qv.newstarts.cn

Ruby: arr.include?(x)
来源：http://ue.hnjuh.cn

C#:   list.Contains(x)
来源：http://xz.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://qx.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aw.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gh.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ys.newstarts.cn

TS:   [...arr];
来源：http://vx.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://bt.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://av.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://qo.shxzskj.cn

C#:   new List<int>(list);
来源：http://oo.huixiangedu.cn

[D23] reduce 累积计算
来源：http://dp.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fq.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kc.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xh.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ra.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ii.521024.cn

Go:   // 手写循环
来源：http://ea.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hn.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yp.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://ry.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mz.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wc.bookmarksfly.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zn.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dv.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ch.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bp.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lk.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mn.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://uu.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jh.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tr.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qn.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xe.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bq.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zd.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hx.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sm.muxihuayi.cn

[D26] 数组转字符串
来源：http://rk.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://nr.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://fa.haigaiapp.cn

JS:   arr.join(", ")
来源：http://ib.hnjuh.cn

TS:   arr.join(", ")
来源：http://np.nszjky.cn


<!-- 参考信息 -->