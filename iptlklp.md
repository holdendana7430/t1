代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sw.shxzskj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tg.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jn.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mu.muxihuayi.cn

[C10] 变量作用域
来源：http://ws.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gd.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lp.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://of.nszjky.cn

TS:   同 JS
来源：http://kv.newstarts.cn

Java: 方法内为块级作用域
来源：http://ha.shtwfgs.cn

Go:   花括号块级作用域
来源：http://du.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tg.bookmarksfly.cn

C#:   块级作用域
来源：http://jj.yuexingan06.cn

[C11] 模块导入与导出
来源：http://by.shxzukj.cn

Py:   from module import func
来源：http://sl.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jh.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pl.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ib.jianghongdianzi.cn

Java: import java.util.List;
来源：http://jn.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sj.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://qb.panjiajie.cn

C#:   using System.Text;
来源：http://ue.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://aj.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://rl.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://mr.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://ew.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://ci.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ae.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://ym.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://ct.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uq.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://xo.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ra.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tx.521024.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iw.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mj.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ge.szsharing.cn

Go:   func add(a, b int) int
来源：http://jf.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cn.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bt.yuntaijiaju.cn

[C14] 泛型函数
来源：http://os.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rj.colortex.cn

PHP:  // 无泛型
来源：http://zh.szxytkj.cn

JS:   // 无泛型
来源：http://dw.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qt.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lu.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fe.huanxung.cn

Ruby: # 无泛型
来源：http://ia.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://su.colortex.cn

[C15] 解构 / 展开参数
来源：http://gk.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://my.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://gh.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vv.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wj.wgjwhj.cn

Java: // 无解构
来源：http://ih.gzmigu.cn

Go:   // 无解构
来源：http://jl.szsharing.cn

Ruby: a, b = pair
来源：http://fe.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://nm.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://zs.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jd.haigaiapp.cn

PHP:  // 无重载
来源：http://zv.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ec.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://mu.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hg.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://nj.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://ks.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fm.jianghongdianzi.cn

================================================================================
来源：http://sr.colortex.cn

D. 数组 / 列表 / 集合
来源：http://fs.asd995.cn

================================================================================
来源：http://ft.521024.cn

[D01] 创建数组 / 列表
来源：http://rb.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cr.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wg.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vk.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://va.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qr.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://xo.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://bp.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rv.shxzskj.cn

[D02] 追加元素到末尾
来源：http://xr.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xw.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vm.chemitech.net.cn

JS:   arr.push(4);
来源：http://xt.szsharing.cn

TS:   arr.push(4);
来源：http://nd.nicolike.cn

Java: list.add(4);
来源：http://uu.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://mx.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://li.muxihuayi.cn

C#:   list.Add(4);
来源：http://ab.nicolike.cn

[D03] 在指定位置插入元素
来源：http://cy.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://rz.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jk.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rz.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://zt.shxzukj.cn

Java: list.add(0, 0);
来源：http://kh.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hc.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bq.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://oo.newstarts.cn

[D04] 删除元素
来源：http://tx.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ic.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jq.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kl.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://gq.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://au.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yb.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wb.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://of.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://mq.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://il.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sw.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sy.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://xu.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://ib.bjjhwx.cn

Go:   arr[0]; arr[0] = 9
来源：http://kb.asd995.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lv.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yi.gzmigu.cn

[D06] 数组长度
来源：http://vm.shtwfgs.cn

Py:   len(arr)
来源：http://sq.jctech888.com.cn

PHP:  count($arr);
来源：http://zj.asd995.cn

JS:   arr.length
来源：http://aa.hahajie.cn

TS:   arr.length
来源：http://uy.szxytkj.cn

Java: list.size();
来源：http://bh.nszjky.cn

Go:   len(arr)
来源：http://ft.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://ml.bjjhwx.cn

C#:   list.Count;
来源：http://ed.nicolike.cn

[D07] 切片 / 取子数组
来源：http://lh.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ve.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ov.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://pu.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://yu.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://nn.shtwfgs.cn

Go:   arr[1:4]
来源：http://ry.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://nx.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://dp.asd995.cn

[D08] 合并两个数组
来源：http://ut.521024.cn

Py:   a + b;  a.extend(b)
来源：http://fx.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://eq.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://li.haigaiapp.cn

TS:   [...a, ...b];
来源：http://wm.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hb.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://uq.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://tb.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://pi.jctech888.com.cn

[D09] 排序（升序）
来源：http://og.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://kh.muxihuayi.cn

PHP:  sort($arr);
来源：http://ts.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wj.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vu.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cw.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iw.lnxyls.cn

Ruby: arr.sort
来源：http://vz.521024.cn

C#:   list.Sort();
来源：http://wt.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qp.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ue.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://az.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rv.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hw.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zk.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dz.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ra.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nn.huanxung.cn

[D11] 反转数组
来源：http://rn.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xc.521024.cn

PHP:  array_reverse($arr);
来源：http://zd.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zm.newstarts.cn

TS:   [...arr].reverse();
来源：http://qc.huanxung.cn

Java: Collections.reverse(list);
来源：http://ok.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://tq.521024.cn

Ruby: arr.reverse
来源：http://qy.shxzukj.cn

C#:   list.Reverse();
来源：http://ki.szsharing.cn

[D12] 查找元素下标
来源：http://vf.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://uf.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vh.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ch.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qo.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gi.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://gu.haigaiapp.cn

Ruby: arr.index(x)
来源：http://ko.hahajie.cn

C#:   list.IndexOf(x);
来源：http://ul.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://me.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tm.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ix.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://ff.szsharing.cn

TS:   arr.filter(x => x > 3)
来源：http://bw.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bu.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jg.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ce.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qt.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://hg.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nj.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ti.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://we.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://lx.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://av.muxihuayi.cn

Go:   // 手写循环
来源：http://gb.muxihuayi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://av.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zw.colortex.cn

[D15] 去重
来源：http://la.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dr.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://zo.huanxung.cn

JS:   [...new Set(arr)]
来源：http://gw.asd995.cn

TS:   [...new Set(arr)]
来源：http://yh.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kd.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://us.hnjuh.cn

Ruby: arr.uniq
来源：http://to.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://qo.bjjhwx.cn

[D16] 求和与平均值
来源：http://ki.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nn.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tm.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://db.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gp.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sf.szsharing.cn

Go:   // 手写循环累加
来源：http://wz.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qw.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://um.huanxung.cn

[D17] 最大值与最小值
来源：http://me.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://xf.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://fd.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xm.newstarts.cn

TS:   Math.max(...arr);
来源：http://yw.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tj.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sm.521024.cn

Ruby: arr.max;  arr.min
来源：http://yc.asd995.cn

C#:   list.Max();  list.Min()
来源：http://uh.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://fl.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ol.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://hr.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://et.9csxet.cn

TS:   nested.flat();
来源：http://hp.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bo.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://ms.shxzukj.cn

Ruby: nested.flatten
来源：http://ps.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ha.muxihuayi.cn

[D19] 按字段分组
来源：http://pg.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zd.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sq.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://th.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cu.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lg.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://sc.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://in.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ka.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://zv.yuexingan06.cn

Py:   Counter(arr)
来源：http://qw.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://nq.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ay.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sb.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ig.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://tl.panjiajie.cn

Ruby: arr.tally
来源：http://bp.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ph.nicolike.cn

[D21] 判断是否包含某元素
来源：http://el.muxihuayi.cn

Py:   x in arr
来源：http://ui.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://pn.shtwfgs.cn

JS:   arr.includes(x)
来源：http://bm.nszjky.cn

TS:   arr.includes(x)
来源：http://hv.nszjky.cn

Java: list.contains(x)
来源：http://jt.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://om.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://hg.huixiangedu.cn

C#:   list.Contains(x)
来源：http://pb.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://nc.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kg.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dw.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iy.asd995.cn

TS:   [...arr];
来源：http://wq.szsharing.cn

Java: new ArrayList<>(list);
来源：http://ux.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fb.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://vx.jianghongdianzi.cn

C#:   new List<int>(list);
来源：http://mt.yuexingan06.cn

[D23] reduce 累积计算
来源：http://wa.yuntaijiaju.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ux.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ls.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vl.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cc.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://li.hnjuh.cn

Go:   // 手写循环
来源：http://cs.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://co.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://il.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://jf.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yw.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gk.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nq.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pi.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gm.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://og.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yv.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wr.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://fr.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xt.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ri.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ts.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qe.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nj.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bb.shxzukj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sy.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mk.szxytkj.cn

[D26] 数组转字符串
来源：http://up.shtwfgs.cn

Py:   ", ".join(map(str, arr))
来源：http://vt.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://zk.haigaiapp.cn

JS:   arr.join(", ")
来源：http://im.huixiangedu.cn

TS:   arr.join(", ")
来源：http://sf.jctech888.com.cn


<!-- 参考信息 -->