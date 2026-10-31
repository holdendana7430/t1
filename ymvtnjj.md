代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fg.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mb.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xu.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xa.panjiajie.cn

[C10] 变量作用域
来源：http://ln.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xd.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pn.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jo.521024.cn

TS:   同 JS
来源：http://jd.szsharing.cn

Java: 方法内为块级作用域
来源：http://jd.hnjuh.cn

Go:   花括号块级作用域
来源：http://zx.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ek.colortex.cn

C#:   块级作用域
来源：http://rv.shxzskj.cn

[C11] 模块导入与导出
来源：http://cm.szsharing.cn

Py:   from module import func
来源：http://qy.yuntaijiaju.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gw.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mf.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rt.nicolike.cn

Java: import java.util.List;
来源：http://yv.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bs.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://ay.yuntaijiaju.cn

C#:   using System.Text;
来源：http://er.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://di.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://rx.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://vv.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://da.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://oo.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ve.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://aw.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://lt.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hj.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://vm.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vw.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wd.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ui.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://za.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jw.521024.cn

Go:   func add(a, b int) int
来源：http://ui.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tb.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qb.huanxung.cn

[C14] 泛型函数
来源：http://yj.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lp.hnjuh.cn

PHP:  // 无泛型
来源：http://pa.huixiangedu.cn

JS:   // 无泛型
来源：http://jd.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://br.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qz.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nt.bookmarksfly.cn

Ruby: # 无泛型
来源：http://tq.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://od.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://fn.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ud.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://vx.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qy.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jn.wgjwhj.cn

Java: // 无解构
来源：http://ox.nszjky.cn

Go:   // 无解构
来源：http://xi.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://na.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://ar.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://ab.szsharing.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ht.shtwfgs.cn

PHP:  // 无重载
来源：http://et.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vp.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://yo.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hm.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://lz.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://uq.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://el.szxytkj.cn

================================================================================
来源：http://jk.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://hm.yuntaijiaju.cn

================================================================================
来源：http://ju.newstarts.cn

[D01] 创建数组 / 列表
来源：http://jv.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vx.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wu.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ug.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zh.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nk.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://gq.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://ls.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vv.gzmigu.cn

[D02] 追加元素到末尾
来源：http://ss.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fl.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ae.wgjwhj.cn

JS:   arr.push(4);
来源：http://yp.muxihuayi.cn

TS:   arr.push(4);
来源：http://jx.nszjky.cn

Java: list.add(4);
来源：http://zr.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://tk.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://ck.lnxyls.cn

C#:   list.Add(4);
来源：http://wo.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://cg.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://ef.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tr.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wi.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://pq.jctech888.com.cn

Java: list.add(0, 0);
来源：http://wz.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kg.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nj.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://fd.muxihuayi.cn

[D04] 删除元素
来源：http://ys.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xx.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gb.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fg.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://nd.bookmarksfly.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hm.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lr.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://in.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gm.9csxet.cn

[D05] 访问与修改元素
来源：http://ch.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eo.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hm.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ve.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://ki.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://yy.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://kn.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fi.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nh.yuexingan06.cn

[D06] 数组长度
来源：http://lg.521024.cn

Py:   len(arr)
来源：http://ws.huixiangedu.cn

PHP:  count($arr);
来源：http://ya.hnjuh.cn

JS:   arr.length
来源：http://xv.nicolike.cn

TS:   arr.length
来源：http://jo.szxytkj.cn

Java: list.size();
来源：http://gb.jctech888.com.cn

Go:   len(arr)
来源：http://hh.newstarts.cn

Ruby: arr.length; arr.size
来源：http://rf.shtwfgs.cn

C#:   list.Count;
来源：http://ef.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://ae.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fd.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gw.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://ff.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://db.szsharing.cn

Java: list.subList(1, 4);
来源：http://tj.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://dh.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://bk.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://rz.colortex.cn

[D08] 合并两个数组
来源：http://qb.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://ho.colortex.cn

PHP:  array_merge($a, $b);
来源：http://cf.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ko.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://hy.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zv.colortex.cn

Go:   append(a, b...)
来源：http://qn.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://fi.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://yo.bjjhwx.cn

[D09] 排序（升序）
来源：http://he.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://rt.huixinmuqiang.cn

PHP:  sort($arr);
来源：http://lo.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jv.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://le.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cy.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oc.gzmigu.cn

Ruby: arr.sort
来源：http://aa.hnjuh.cn

C#:   list.Sort();
来源：http://ak.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hm.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kz.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nu.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gl.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mg.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dn.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yr.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gs.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zz.jianghongdianzi.cn

[D11] 反转数组
来源：http://jp.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yl.nszjky.cn

PHP:  array_reverse($arr);
来源：http://le.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wa.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://cy.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://hj.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://nr.bjjhwx.cn

Ruby: arr.reverse
来源：http://ya.9csxet.cn

C#:   list.Reverse();
来源：http://sl.szsharing.cn

[D12] 查找元素下标
来源：http://ef.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://wl.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ci.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bi.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pd.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uh.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://wj.shxzskj.cn

Ruby: arr.index(x)
来源：http://jl.hahajie.cn

C#:   list.IndexOf(x);
来源：http://hb.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://qj.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ui.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zn.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://be.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://xu.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vq.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yn.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cb.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ki.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://iu.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qq.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gw.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://ej.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://cn.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ac.colortex.cn

Go:   // 手写循环
来源：http://nr.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yt.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nf.521024.cn

[D15] 去重
来源：http://fg.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jt.szsharing.cn

PHP:  array_unique($arr);
来源：http://vb.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://rn.9csxet.cn

TS:   [...new Set(arr)]
来源：http://ap.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cd.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nw.hahajie.cn

Ruby: arr.uniq
来源：http://zl.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://qo.muxihuayi.cn

[D16] 求和与平均值
来源：http://rl.muxihuayi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bo.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qt.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mv.chemitech.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wn.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rb.yuexingan06.cn

Go:   // 手写循环累加
来源：http://bm.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jj.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://fc.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://mz.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://dn.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://nu.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nn.9csxet.cn

TS:   Math.max(...arr);
来源：http://ox.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ot.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oy.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://hn.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://nr.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://fv.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gq.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://mm.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gq.bjjhwx.cn

TS:   nested.flat();
来源：http://xf.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hy.chemitech.net.cn

Go:   // 手写双层循环
来源：http://dg.jctech888.com.cn

Ruby: nested.flatten
来源：http://zn.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lg.jctech888.com.cn

[D19] 按字段分组
来源：http://vu.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ya.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nl.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tg.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cq.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dn.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://lv.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jt.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bo.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://nr.chemitech.net.cn

Py:   Counter(arr)
来源：http://xy.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://pw.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uj.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yn.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dt.hahajie.cn

Go:   // 手写 map[T]int
来源：http://je.huanxung.cn

Ruby: arr.tally
来源：http://vy.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ka.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://la.yuexingan06.cn

Py:   x in arr
来源：http://xo.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://id.szxytkj.cn

JS:   arr.includes(x)
来源：http://gk.huanxung.cn

TS:   arr.includes(x)
来源：http://pi.yuntaijiaju.cn

Java: list.contains(x)
来源：http://of.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://ok.newstarts.cn

Ruby: arr.include?(x)
来源：http://em.newstarts.cn

C#:   list.Contains(x)
来源：http://vv.shxzskj.cn

[D22] 复制数组（避免共享引用）
来源：http://he.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cq.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tk.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rl.yuntaijiaju.cn

TS:   [...arr];
来源：http://da.nicolike.cn

Java: new ArrayList<>(list);
来源：http://gy.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gm.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://nj.colortex.cn

C#:   new List<int>(list);
来源：http://kd.szsharing.cn

[D23] reduce 累积计算
来源：http://xg.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nh.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gv.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ti.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cr.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xs.bjjhwx.cn

Go:   // 手写循环
来源：http://dr.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rv.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gu.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://ey.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ns.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yn.huixinmuqiang.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ll.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dy.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gn.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yu.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fq.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lp.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://zs.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pp.521024.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jp.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ax.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://km.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ir.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oa.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xt.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jc.nicolike.cn

[D26] 数组转字符串
来源：http://kd.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://hw.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://cf.wgjwhj.cn

JS:   arr.join(", ")
来源：http://np.haigaiapp.cn

TS:   arr.join(", ")
来源：http://co.shtwfgs.cn


<!-- 参考信息 -->