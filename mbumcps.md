代发 wailian999

C#:   块级作用域
来源：http://mf.shtwfgs.cn

[C11] 模块导入与导出
来源：http://ap.szxytkj.cn

Py:   from module import func
来源：http://pv.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ry.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://en.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://by.shxzskj.cn

Java: import java.util.List;
来源：http://ig.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sy.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://zl.hahajie.cn

C#:   using System.Text;
来源：http://vw.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://zt.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://wr.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://pq.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://qe.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://lq.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ge.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://qu.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://qe.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ao.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://nh.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mq.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wj.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ff.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wp.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tt.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://xt.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eo.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nj.huanxung.cn

[C14] 泛型函数
来源：http://za.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sl.shxzukj.cn

PHP:  // 无泛型
来源：http://dd.jianghongdianzi.cn

JS:   // 无泛型
来源：http://dw.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ar.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dw.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aj.wgjwhj.cn

Ruby: # 无泛型
来源：http://ti.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aw.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://qw.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ja.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://dy.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://no.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://us.shxzukj.cn

Java: // 无解构
来源：http://hw.wgjwhj.cn

Go:   // 无解构
来源：http://tl.nszjky.cn

Ruby: a, b = pair
来源：http://tf.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://ys.szsharing.cn

[C16] 函数 / 方法重载
来源：http://gq.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ti.wgjwhj.cn

PHP:  // 无重载
来源：http://av.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sf.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://hr.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://di.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://ft.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://ih.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ip.szsharing.cn

================================================================================
来源：http://ak.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://ox.asd995.cn

================================================================================
来源：http://vf.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://sd.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nv.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jh.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zl.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hr.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nm.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://iw.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://jl.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fr.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://cf.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kg.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ku.hnjuh.cn

JS:   arr.push(4);
来源：http://as.szsharing.cn

TS:   arr.push(4);
来源：http://ic.nicolike.cn

Java: list.add(4);
来源：http://po.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://hf.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://xf.nszjky.cn

C#:   list.Add(4);
来源：http://gl.9csxet.cn

[D03] 在指定位置插入元素
来源：http://aj.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://zf.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wp.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oa.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://fs.muxihuayi.cn

Java: list.add(0, 0);
来源：http://lg.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ar.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ah.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://vl.szxytkj.cn

[D04] 删除元素
来源：http://de.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ys.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bf.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rs.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://xf.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tu.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mr.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aa.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ds.huixiangedu.cn

[D05] 访问与修改元素
来源：http://tz.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uz.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wr.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fp.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://td.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://vw.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://tw.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qk.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hr.9csxet.cn

[D06] 数组长度
来源：http://ph.521024.cn

Py:   len(arr)
来源：http://gn.newstarts.cn

PHP:  count($arr);
来源：http://my.shxzskj.cn

JS:   arr.length
来源：http://yq.chemitech.net.cn

TS:   arr.length
来源：http://jt.9csxet.cn

Java: list.size();
来源：http://db.lnxyls.cn

Go:   len(arr)
来源：http://rd.hahajie.cn

Ruby: arr.length; arr.size
来源：http://bk.hahajie.cn

C#:   list.Count;
来源：http://ia.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://ih.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dw.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xe.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://fp.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://rn.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://jj.newstarts.cn

Go:   arr[1:4]
来源：http://um.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://iw.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://ev.panjiajie.cn

[D08] 合并两个数组
来源：http://pm.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://vq.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://st.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fh.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://bj.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fp.nszjky.cn

Go:   append(a, b...)
来源：http://bd.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://mf.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://gk.shtwfgs.cn

[D09] 排序（升序）
来源：http://ip.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://nj.nicolike.cn

PHP:  sort($arr);
来源：http://xn.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sk.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gx.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sf.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yj.huanxung.cn

Ruby: arr.sort
来源：http://gf.szsharing.cn

C#:   list.Sort();
来源：http://ob.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://an.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fr.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yr.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cr.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rz.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gh.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lx.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ll.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rl.shtwfgs.cn

[D11] 反转数组
来源：http://qj.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xs.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://os.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://io.521024.cn

TS:   [...arr].reverse();
来源：http://pn.hahajie.cn

Java: Collections.reverse(list);
来源：http://pt.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://im.szxytkj.cn

Ruby: arr.reverse
来源：http://ju.gzmigu.cn

C#:   list.Reverse();
来源：http://ij.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://js.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://lq.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tt.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bd.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qb.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wd.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://kk.newstarts.cn

Ruby: arr.index(x)
来源：http://em.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://zz.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://kw.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gk.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qj.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://bs.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://oj.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dq.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cy.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://be.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ep.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://vu.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uo.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sg.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://xn.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://lo.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://po.szxytkj.cn

Go:   // 手写循环
来源：http://qc.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cr.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tm.yuexingan06.cn

[D15] 去重
来源：http://ko.muxihuayi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nk.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://fc.nszjky.cn

JS:   [...new Set(arr)]
来源：http://ay.szsharing.cn

TS:   [...new Set(arr)]
来源：http://pr.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wq.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fv.bjjhwx.cn

Ruby: arr.uniq
来源：http://hx.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://up.shxzskj.cn

[D16] 求和与平均值
来源：http://yv.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dg.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vk.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wb.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lh.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cr.nszjky.cn

Go:   // 手写循环累加
来源：http://tr.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vu.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://yc.521024.cn

[D17] 最大值与最小值
来源：http://zp.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://rb.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://ex.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cg.bookmarksfly.cn

TS:   Math.max(...arr);
来源：http://xa.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ft.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jy.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://uz.colortex.cn

C#:   list.Max();  list.Min()
来源：http://dz.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://fg.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://li.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://ke.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lv.bookmarksfly.cn

TS:   nested.flat();
来源：http://vo.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hnjuh.cn

Go:   // 手写双层循环
来源：http://lk.shxzskj.cn

Ruby: nested.flatten
来源：http://iq.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ua.nicolike.cn

[D19] 按字段分组
来源：http://rz.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cy.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qq.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bg.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oq.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ck.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://hw.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hl.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xy.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://kg.jctech888.com.cn

Py:   Counter(arr)
来源：http://mu.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://be.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ft.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gj.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kl.nicolike.cn

Go:   // 手写 map[T]int
来源：http://jq.yuntaijiaju.cn

Ruby: arr.tally
来源：http://hw.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gc.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://az.szxytkj.cn

Py:   x in arr
来源：http://la.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://du.nicolike.cn

JS:   arr.includes(x)
来源：http://ai.muxihuayi.cn

TS:   arr.includes(x)
来源：http://sx.szsharing.cn

Java: list.contains(x)
来源：http://tm.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://pd.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://su.wgjwhj.cn

C#:   list.Contains(x)
来源：http://eh.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://ui.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dl.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://li.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ip.muxihuayi.cn

TS:   [...arr];
来源：http://xu.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://jt.szxytkj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yh.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://kf.colortex.cn

C#:   new List<int>(list);
来源：http://yz.muxihuayi.cn

[D23] reduce 累积计算
来源：http://dh.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hi.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gg.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vx.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ev.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qy.lnxyls.cn

Go:   // 手写循环
来源：http://in.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mf.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pm.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://qw.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oc.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aq.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ix.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://js.shxzukj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hi.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wa.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://av.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sf.521024.cn

[D25] Set 集合去重与交并差
来源：http://og.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ic.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ha.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ef.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qn.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xy.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ay.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fe.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://va.colortex.cn

[D26] 数组转字符串
来源：http://ug.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://pu.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://dd.panjiajie.cn

JS:   arr.join(", ")
来源：http://df.hnjuh.cn

TS:   arr.join(", ")
来源：http://nh.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://ni.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://gn.lnxyls.cn

Ruby: arr.join(", ")
来源：http://nn.nszjky.cn

C#:   string.Join(", ", list)
来源：http://vy.szsharing.cn

================================================================================
来源：http://xx.hnjuh.cn

E. 字符串处理
来源：http://er.hnjuh.cn

================================================================================
来源：http://xh.521024.cn

[E01] 拼接字符串
来源：http://ck.521024.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ce.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iq.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rz.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aa.huixinmuqiang.cn


<!-- 参考信息 -->