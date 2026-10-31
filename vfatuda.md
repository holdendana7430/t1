代发 wailian999

[C10] 变量作用域
来源：http://bk.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rb.bookmarksfly.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nr.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ok.lnxyls.cn

TS:   同 JS
来源：http://la.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://zf.muxihuayi.cn

Go:   花括号块级作用域
来源：http://hy.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qx.bookmarksfly.cn

C#:   块级作用域
来源：http://ag.asd995.cn

[C11] 模块导入与导出
来源：http://yu.shxzukj.cn

Py:   from module import func
来源：http://bn.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://da.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dy.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nm.muxihuayi.cn

Java: import java.util.List;
来源：http://po.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jr.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://bl.wgjwhj.cn

C#:   using System.Text;
来源：http://eb.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://pj.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://ql.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://rm.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://fl.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://gm.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fw.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://nv.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://pq.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wa.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://wj.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mw.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mc.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fw.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ma.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ps.newstarts.cn

Go:   func add(a, b int) int
来源：http://kd.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wj.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lw.shxzskj.cn

[C14] 泛型函数
来源：http://zu.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://um.huixiangedu.cn

PHP:  // 无泛型
来源：http://dn.huixinmuqiang.cn

JS:   // 无泛型
来源：http://ny.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dp.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nw.szxytkj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xq.lnxyls.cn

Ruby: # 无泛型
来源：http://vk.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ob.nszjky.cn

[C15] 解构 / 展开参数
来源：http://jx.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zc.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://lt.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kg.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://li.colortex.cn

Java: // 无解构
来源：http://cp.yuexingan06.cn

Go:   // 无解构
来源：http://bo.colortex.cn

Ruby: a, b = pair
来源：http://av.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://hm.9csxet.cn

[C16] 函数 / 方法重载
来源：http://dk.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vi.colortex.cn

PHP:  // 无重载
来源：http://ap.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hd.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://if.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ip.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://wn.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://yl.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ue.yuexingan06.cn

================================================================================
来源：http://ql.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://ve.shxzskj.cn

================================================================================
来源：http://fm.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://vn.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ck.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://au.jianghongdianzi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xl.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vj.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wd.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://tn.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://qk.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ud.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://ji.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iq.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ug.yuexingan06.cn

JS:   arr.push(4);
来源：http://gf.newstarts.cn

TS:   arr.push(4);
来源：http://qf.yuexingan06.cn

Java: list.add(4);
来源：http://ze.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://ky.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://ev.wgjwhj.cn

C#:   list.Add(4);
来源：http://vo.hahajie.cn

[D03] 在指定位置插入元素
来源：http://cv.colortex.cn

Py:   arr.insert(0, 0)
来源：http://mr.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kb.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pz.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://oi.hahajie.cn

Java: list.add(0, 0);
来源：http://oa.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://at.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wx.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://iw.gzmigu.cn

[D04] 删除元素
来源：http://wv.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dj.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uo.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qt.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://hj.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lw.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mq.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mj.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nw.wgjwhj.cn

[D05] 访问与修改元素
来源：http://xs.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jf.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pd.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xg.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://mg.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://oy.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://og.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ku.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sw.jctech888.com.cn

[D06] 数组长度
来源：http://vy.shxzukj.cn

Py:   len(arr)
来源：http://ja.nicolike.cn

PHP:  count($arr);
来源：http://dt.521024.cn

JS:   arr.length
来源：http://cj.huixinmuqiang.cn

TS:   arr.length
来源：http://qz.newstarts.cn

Java: list.size();
来源：http://pr.gzmigu.cn

Go:   len(arr)
来源：http://yr.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://ns.chemitech.net.cn

C#:   list.Count;
来源：http://pp.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://dd.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ez.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uj.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://lv.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://np.panjiajie.cn

Java: list.subList(1, 4);
来源：http://hl.asd995.cn

Go:   arr[1:4]
来源：http://mr.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://oh.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://te.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://lg.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://nh.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://fk.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uh.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://ur.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gc.chemitech.net.cn

Go:   append(a, b...)
来源：http://ul.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://ju.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://zn.wgjwhj.cn

[D09] 排序（升序）
来源：http://ig.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://kn.yuexingan06.cn

PHP:  sort($arr);
来源：http://hf.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xx.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vp.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fm.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://st.shxzskj.cn

Ruby: arr.sort
来源：http://rl.huixiangedu.cn

C#:   list.Sort();
来源：http://zv.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vw.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xd.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ga.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sf.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wb.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yk.lnxyls.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fd.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lz.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hv.nicolike.cn

[D11] 反转数组
来源：http://tr.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kj.colortex.cn

PHP:  array_reverse($arr);
来源：http://ht.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dy.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://gb.szxytkj.cn

Java: Collections.reverse(list);
来源：http://fz.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://ho.bjjhwx.cn

Ruby: arr.reverse
来源：http://ze.shxzukj.cn

C#:   list.Reverse();
来源：http://pz.shxzskj.cn

[D12] 查找元素下标
来源：http://li.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://cq.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oy.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fo.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pc.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://as.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://na.chemitech.net.cn

Ruby: arr.index(x)
来源：http://xb.asd995.cn

C#:   list.IndexOf(x);
来源：http://qo.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://fu.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kz.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cx.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://uf.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://ne.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ku.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qe.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ep.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sf.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://hj.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mo.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qz.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://vj.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://ip.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bb.chemitech.net.cn

Go:   // 手写循环
来源：http://kt.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nf.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zs.yuntaijiaju.cn

[D15] 去重
来源：http://ks.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cb.colortex.cn

PHP:  array_unique($arr);
来源：http://uw.9csxet.cn

JS:   [...new Set(arr)]
来源：http://lq.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://xe.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zx.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dg.asd995.cn

Ruby: arr.uniq
来源：http://cp.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://iq.huixiangedu.cn

[D16] 求和与平均值
来源：http://ss.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uh.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ww.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bu.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ni.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tn.huanxung.cn

Go:   // 手写循环累加
来源：http://cc.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lg.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://qo.colortex.cn

[D17] 最大值与最小值
来源：http://bx.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://mx.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://ao.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rv.panjiajie.cn

TS:   Math.max(...arr);
来源：http://nq.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ug.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ph.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://gi.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://gj.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://om.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vj.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://si.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jz.521024.cn

TS:   nested.flat();
来源：http://nw.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yr.jctech888.com.cn

Go:   // 手写双层循环
来源：http://ob.nicolike.cn

Ruby: nested.flatten
来源：http://qs.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ct.lnxyls.cn

[D19] 按字段分组
来源：http://fx.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eb.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nz.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tz.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qf.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ch.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://pg.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ct.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ls.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://vb.shxzukj.cn

Py:   Counter(arr)
来源：http://da.nicolike.cn

PHP:  array_count_values($arr);
来源：http://xd.shxzukj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rq.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vf.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oc.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://lf.haigaiapp.cn

Ruby: arr.tally
来源：http://jx.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ot.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://hz.lnxyls.cn

Py:   x in arr
来源：http://fs.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://hl.yuexingan06.cn

JS:   arr.includes(x)
来源：http://wm.nicolike.cn

TS:   arr.includes(x)
来源：http://pe.asd995.cn

Java: list.contains(x)
来源：http://ez.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://qp.shxzskj.cn

Ruby: arr.include?(x)
来源：http://be.nszjky.cn

C#:   list.Contains(x)
来源：http://nn.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://qm.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dn.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ol.huixiangedu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jh.hahajie.cn

TS:   [...arr];
来源：http://er.newstarts.cn

Java: new ArrayList<>(list);
来源：http://ry.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vf.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://zv.shxzukj.cn

C#:   new List<int>(list);
来源：http://dg.shxzskj.cn

[D23] reduce 累积计算
来源：http://kx.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pz.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rb.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jr.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jg.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://us.521024.cn

Go:   // 手写循环
来源：http://nr.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gd.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pt.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://dz.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ma.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nd.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uo.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nj.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mj.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ba.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nx.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bp.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://ku.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rj.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xn.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://av.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wy.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oo.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sn.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wm.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oz.bjjhwx.cn

[D26] 数组转字符串
来源：http://lx.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://hj.jctech888.com.cn

PHP:  implode(", ", $arr);
来源：http://aa.hnjuh.cn

JS:   arr.join(", ")
来源：http://fo.haigaiapp.cn

TS:   arr.join(", ")
来源：http://ci.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://fd.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://uv.newstarts.cn

Ruby: arr.join(", ")
来源：http://qy.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://xf.panjiajie.cn


<!-- 参考信息 -->