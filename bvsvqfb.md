代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rh.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ko.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yv.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://da.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pv.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qs.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fa.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://di.hnjuh.cn

[C10] 变量作用域
来源：http://nw.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bt.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yq.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://af.szsharing.cn

TS:   同 JS
来源：http://ga.nicolike.cn

Java: 方法内为块级作用域
来源：http://ri.9csxet.cn

Go:   花括号块级作用域
来源：http://iq.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fq.szxytkj.cn

C#:   块级作用域
来源：http://ec.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://jb.szxytkj.cn

Py:   from module import func
来源：http://mv.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bw.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fd.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qg.shtwfgs.cn

Java: import java.util.List;
来源：http://ha.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rf.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://fh.wgjwhj.cn

C#:   using System.Text;
来源：http://nh.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://vi.lnxyls.cn

Py:   (lambda: print("run"))()
来源：http://oi.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://gq.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://ok.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://ow.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mb.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://mo.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://vi.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rx.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://lq.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lf.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://es.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gf.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gj.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lt.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://xz.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uu.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vj.hahajie.cn

[C14] 泛型函数
来源：http://ro.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tr.gzmigu.cn

PHP:  // 无泛型
来源：http://vo.bjjhwx.cn

JS:   // 无泛型
来源：http://ku.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jv.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gq.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://is.chemitech.net.cn

Ruby: # 无泛型
来源：http://fb.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dj.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://me.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cd.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://av.asd995.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ot.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bn.newstarts.cn

Java: // 无解构
来源：http://up.asd995.cn

Go:   // 无解构
来源：http://jy.colortex.cn

Ruby: a, b = pair
来源：http://zp.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://nu.shxzukj.cn

[C16] 函数 / 方法重载
来源：http://il.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bn.jctech888.com.cn

PHP:  // 无重载
来源：http://as.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ii.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://pj.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xf.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://rv.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://qq.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fb.colortex.cn

================================================================================
来源：http://ik.asd995.cn

D. 数组 / 列表 / 集合
来源：http://au.panjiajie.cn

================================================================================
来源：http://nb.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://qz.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xj.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sy.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yo.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kf.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://na.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://yx.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://nm.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tu.shxzukj.cn

[D02] 追加元素到末尾
来源：http://cl.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vh.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tp.newstarts.cn

JS:   arr.push(4);
来源：http://ke.yuexingan06.cn

TS:   arr.push(4);
来源：http://kr.asd995.cn

Java: list.add(4);
来源：http://wz.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://kv.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://ho.huanxung.cn

C#:   list.Add(4);
来源：http://ej.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://no.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://my.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cx.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bc.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://yc.bjjhwx.cn

Java: list.add(0, 0);
来源：http://qz.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fz.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ny.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://nz.szxytkj.cn

[D04] 删除元素
来源：http://vk.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ok.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://da.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dk.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://wm.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jj.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dp.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ow.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xv.chemitech.net.cn

[D05] 访问与修改元素
来源：http://fy.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sw.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qd.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://or.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://ae.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://wm.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://dy.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yg.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tk.9csxet.cn

[D06] 数组长度
来源：http://ek.muxihuayi.cn

Py:   len(arr)
来源：http://ew.hahajie.cn

PHP:  count($arr);
来源：http://sh.yuexingan06.cn

JS:   arr.length
来源：http://dn.wgjwhj.cn

TS:   arr.length
来源：http://rn.szxytkj.cn

Java: list.size();
来源：http://kk.yuntaijiaju.cn

Go:   len(arr)
来源：http://gi.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://ub.hnjuh.cn

C#:   list.Count;
来源：http://ra.huanxung.cn

[D07] 切片 / 取子数组
来源：http://vo.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qe.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://po.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://bh.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://gr.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://wh.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://ug.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://qd.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://yp.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://ok.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://bq.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://kp.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hm.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://gk.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eq.newstarts.cn

Go:   append(a, b...)
来源：http://aa.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://gg.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://rm.lnxyls.cn

[D09] 排序（升序）
来源：http://sn.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://dm.lnxyls.cn

PHP:  sort($arr);
来源：http://ei.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ma.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gk.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hs.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fg.szxytkj.cn

Ruby: arr.sort
来源：http://sg.huixiangedu.cn

C#:   list.Sort();
来源：http://dd.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zz.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ai.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cm.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ns.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hy.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hi.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tn.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vk.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dm.yuexingan06.cn

[D11] 反转数组
来源：http://nw.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fm.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://ns.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gn.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://nt.colortex.cn

Java: Collections.reverse(list);
来源：http://do.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://eh.newstarts.cn

Ruby: arr.reverse
来源：http://ds.colortex.cn

C#:   list.Reverse();
来源：http://eq.colortex.cn

[D12] 查找元素下标
来源：http://ua.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://jf.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sg.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pm.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cv.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aw.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://xk.wgjwhj.cn

Ruby: arr.index(x)
来源：http://aj.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://ul.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://ox.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fd.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dw.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://fq.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://qd.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xy.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kj.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cn.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://io.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://yd.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ab.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ks.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://qk.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://dn.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ep.yuexingan06.cn

Go:   // 手写循环
来源：http://xo.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kh.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hg.huixiangedu.cn

[D15] 去重
来源：http://hy.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cn.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://ew.szsharing.cn

JS:   [...new Set(arr)]
来源：http://gm.nicolike.cn

TS:   [...new Set(arr)]
来源：http://at.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cw.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nc.newstarts.cn

Ruby: arr.uniq
来源：http://dd.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://ko.bjjhwx.cn

[D16] 求和与平均值
来源：http://zg.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zz.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zs.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zo.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gj.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ii.panjiajie.cn

Go:   // 手写循环累加
来源：http://gk.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sp.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://fb.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://ho.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://gf.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://wj.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sw.hahajie.cn

TS:   Math.max(...arr);
来源：http://ob.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ga.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nf.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://pm.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://uj.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://qa.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gs.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://ps.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jd.asd995.cn

TS:   nested.flat();
来源：http://tu.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tm.haigaiapp.cn

Go:   // 手写双层循环
来源：http://wj.chemitech.net.cn

Ruby: nested.flatten
来源：http://hv.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://br.huixiangedu.cn

[D19] 按字段分组
来源：http://sz.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ap.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ow.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hq.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sq.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ev.colortex.cn

Go:   // 手写 map[string][]T
来源：http://cr.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ko.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ih.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://vq.hahajie.cn

Py:   Counter(arr)
来源：http://zf.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://ic.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ji.huixinmuqiang.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fg.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mo.asd995.cn

Go:   // 手写 map[T]int
来源：http://xq.gzmigu.cn

Ruby: arr.tally
来源：http://st.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cb.asd995.cn

[D21] 判断是否包含某元素
来源：http://jn.lnxyls.cn

Py:   x in arr
来源：http://dc.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://um.521024.cn

JS:   arr.includes(x)
来源：http://fk.jctech888.com.cn

TS:   arr.includes(x)
来源：http://gb.hahajie.cn

Java: list.contains(x)
来源：http://cb.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://au.panjiajie.cn

Ruby: arr.include?(x)
来源：http://og.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://id.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://di.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hx.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rf.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sy.haigaiapp.cn

TS:   [...arr];
来源：http://rm.colortex.cn

Java: new ArrayList<>(list);
来源：http://yg.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lq.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://li.521024.cn

C#:   new List<int>(list);
来源：http://mi.colortex.cn

[D23] reduce 累积计算
来源：http://tl.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mp.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pm.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ek.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oh.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zh.hahajie.cn

Go:   // 手写循环
来源：http://ie.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rx.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mg.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://ag.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fi.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ns.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bj.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vv.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://es.9csxet.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mm.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nn.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nq.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://es.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ex.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jw.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xc.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bm.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fh.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zx.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mx.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rj.szsharing.cn

[D26] 数组转字符串
来源：http://jb.colortex.cn


<!-- 参考信息 -->