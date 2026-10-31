代发 wailian999

[C10] 变量作用域
来源：http://fd.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vu.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ag.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oo.9csxet.cn

TS:   同 JS
来源：http://ec.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://ls.nicolike.cn

Go:   花括号块级作用域
来源：http://pf.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ma.muxihuayi.cn

C#:   块级作用域
来源：http://gi.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://lu.lnxyls.cn

Py:   from module import func
来源：http://mk.nicolike.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tv.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kc.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ra.jianghongdianzi.cn

Java: import java.util.List;
来源：http://ks.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vc.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://xa.lnxyls.cn

C#:   using System.Text;
来源：http://xz.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://lk.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://gp.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://nj.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://nl.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://wl.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gn.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://er.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://pj.yuntaijiaju.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tj.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://su.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ql.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mv.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lc.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ln.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cf.szsharing.cn

Go:   func add(a, b int) int
来源：http://ad.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ck.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ko.szsharing.cn

[C14] 泛型函数
来源：http://lv.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gv.gzmigu.cn

PHP:  // 无泛型
来源：http://si.huixiangedu.cn

JS:   // 无泛型
来源：http://wr.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hw.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xn.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sx.colortex.cn

Ruby: # 无泛型
来源：http://nt.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mj.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://ni.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yo.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://tg.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zo.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ud.nszjky.cn

Java: // 无解构
来源：http://lg.colortex.cn

Go:   // 无解构
来源：http://qm.nszjky.cn

Ruby: a, b = pair
来源：http://rl.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://ow.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://ip.colortex.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vw.panjiajie.cn

PHP:  // 无重载
来源：http://zz.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mk.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://bs.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://td.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://iz.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://yv.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://op.shxzskj.cn

================================================================================
来源：http://la.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://qr.huixiangedu.cn

================================================================================
来源：http://xs.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://mh.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ek.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wb.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ua.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://za.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ow.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://cx.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://ng.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qm.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://zt.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cx.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dv.hnjuh.cn

JS:   arr.push(4);
来源：http://ki.huanxung.cn

TS:   arr.push(4);
来源：http://oh.lnxyls.cn

Java: list.add(4);
来源：http://ea.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://ks.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://hs.huixiangedu.cn

C#:   list.Add(4);
来源：http://xy.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://nt.521024.cn

Py:   arr.insert(0, 0)
来源：http://ps.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fe.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gr.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://vc.muxihuayi.cn

Java: list.add(0, 0);
来源：http://su.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://we.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nh.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://dt.hahajie.cn

[D04] 删除元素
来源：http://pi.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fk.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xv.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fv.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://mt.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xb.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xy.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://go.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aq.nszjky.cn

[D05] 访问与修改元素
来源：http://dr.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vi.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://re.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cs.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://qy.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://vy.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://de.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mr.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xv.yuexingan06.cn

[D06] 数组长度
来源：http://yk.jianghongdianzi.cn

Py:   len(arr)
来源：http://oi.yuntaijiaju.cn

PHP:  count($arr);
来源：http://bk.shtwfgs.cn

JS:   arr.length
来源：http://ko.lnxyls.cn

TS:   arr.length
来源：http://on.bjjhwx.cn

Java: list.size();
来源：http://yr.9csxet.cn

Go:   len(arr)
来源：http://uc.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://ns.muxihuayi.cn

C#:   list.Count;
来源：http://mz.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://xi.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://en.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://of.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://pz.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://ms.huixiangedu.cn

Java: list.subList(1, 4);
来源：http://au.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://mw.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://xi.yuexingan06.cn

C#:   list.GetRange(1, 3);
来源：http://uj.newstarts.cn

[D08] 合并两个数组
来源：http://db.521024.cn

Py:   a + b;  a.extend(b)
来源：http://pm.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://if.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rq.huanxung.cn

TS:   [...a, ...b];
来源：http://ta.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xq.szsharing.cn

Go:   append(a, b...)
来源：http://fu.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://qg.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://nz.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://tb.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://ww.asd995.cn

PHP:  sort($arr);
来源：http://ud.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ru.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kf.nszjky.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xe.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ln.szxytkj.cn

Ruby: arr.sort
来源：http://fr.chemitech.net.cn

C#:   list.Sort();
来源：http://gk.newstarts.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wj.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://og.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vk.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cg.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oj.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ub.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lf.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xv.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bn.jianghongdianzi.cn

[D11] 反转数组
来源：http://pa.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uz.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://rj.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bc.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://ew.colortex.cn

Java: Collections.reverse(list);
来源：http://rc.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://qs.521024.cn

Ruby: arr.reverse
来源：http://sw.panjiajie.cn

C#:   list.Reverse();
来源：http://kn.shtwfgs.cn

[D12] 查找元素下标
来源：http://ns.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://lb.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ba.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://td.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://up.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zp.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://bv.nicolike.cn

Ruby: arr.index(x)
来源：http://kq.nicolike.cn

C#:   list.IndexOf(x);
来源：http://wl.nszjky.cn

[D13] 过滤（保留满足条件的）
来源：http://et.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pw.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mf.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://pf.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://tt.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ok.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wb.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mk.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yh.newstarts.cn

[D14] 映射转换（每个元素变形）
来源：http://ps.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yl.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uw.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://oy.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://me.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pn.shtwfgs.cn

Go:   // 手写循环
来源：http://qc.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tv.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ed.jianghongdianzi.cn

[D15] 去重
来源：http://ga.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lz.asd995.cn

PHP:  array_unique($arr);
来源：http://ph.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://xk.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://bx.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ub.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zj.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://ag.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://bg.nszjky.cn

[D16] 求和与平均值
来源：http://ro.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wm.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ox.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ly.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zj.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vx.shtwfgs.cn

Go:   // 手写循环累加
来源：http://ud.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vv.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://ye.panjiajie.cn

[D17] 最大值与最小值
来源：http://ul.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://xy.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://gh.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ir.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://eq.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nj.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://th.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://ok.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://sx.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://fn.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kv.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://pf.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yh.jianghongdianzi.cn

TS:   nested.flat();
来源：http://je.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ix.9csxet.cn

Go:   // 手写双层循环
来源：http://xt.szxytkj.cn

Ruby: nested.flatten
来源：http://ae.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nw.yuntaijiaju.cn

[D19] 按字段分组
来源：http://jd.newstarts.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://us.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wa.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iw.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ka.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ya.521024.cn

Go:   // 手写 map[string][]T
来源：http://iw.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qi.bookmarksfly.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hg.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://uc.chemitech.net.cn

Py:   Counter(arr)
来源：http://ai.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://mf.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cm.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jd.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://go.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://bo.huanxung.cn

Ruby: arr.tally
来源：http://es.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qm.521024.cn

[D21] 判断是否包含某元素
来源：http://sz.yuexingan06.cn

Py:   x in arr
来源：http://oi.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://aq.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://tw.hnjuh.cn

TS:   arr.includes(x)
来源：http://bt.hnjuh.cn

Java: list.contains(x)
来源：http://yq.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://ai.521024.cn

Ruby: arr.include?(x)
来源：http://px.gzmigu.cn

C#:   list.Contains(x)
来源：http://qv.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://tr.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cy.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cr.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xv.shxzukj.cn

TS:   [...arr];
来源：http://qr.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://hm.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ke.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://qt.jctech888.com.cn

C#:   new List<int>(list);
来源：http://vi.huanxung.cn

[D23] reduce 累积计算
来源：http://va.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bf.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xw.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ur.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fo.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://aj.haigaiapp.cn

Go:   // 手写循环
来源：http://gz.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zk.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ua.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://he.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cd.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nz.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cr.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qz.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jq.asd995.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oe.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vj.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mm.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://he.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vj.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ri.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://de.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rl.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nv.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://df.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bx.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nx.hnjuh.cn

[D26] 数组转字符串
来源：http://zy.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://xj.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://an.newstarts.cn

JS:   arr.join(", ")
来源：http://sf.521024.cn

TS:   arr.join(", ")
来源：http://nf.hnjuh.cn

Java: String.join(", ", list)
来源：http://sa.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://wz.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://bc.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://qo.panjiajie.cn


<!-- 参考信息 -->