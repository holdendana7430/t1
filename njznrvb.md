代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bm.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lg.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ug.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gw.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://up.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vn.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yr.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nj.bjjhwx.cn

[C10] 变量作用域
来源：http://ov.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uv.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xx.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qk.shxzskj.cn

TS:   同 JS
来源：http://tv.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://gr.huixiangedu.cn

Go:   花括号块级作用域
来源：http://za.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wd.hnjuh.cn

C#:   块级作用域
来源：http://ga.nszjky.cn

[C11] 模块导入与导出
来源：http://my.gzmigu.cn

Py:   from module import func
来源：http://md.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nc.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wf.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://et.9csxet.cn

Java: import java.util.List;
来源：http://nk.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tt.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://jc.huixinmuqiang.cn

C#:   using System.Text;
来源：http://qm.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://vs.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://sc.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://hk.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://jj.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://ti.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pi.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://xz.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://df.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ab.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://dy.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://es.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pk.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://em.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zu.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ps.panjiajie.cn

Go:   func add(a, b int) int
来源：http://dd.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mz.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qb.bookmarksfly.cn

[C14] 泛型函数
来源：http://uz.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vg.shxzskj.cn

PHP:  // 无泛型
来源：http://ti.wgjwhj.cn

JS:   // 无泛型
来源：http://yg.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lt.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://be.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wd.huixiangedu.cn

Ruby: # 无泛型
来源：http://va.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wq.9csxet.cn

[C15] 解构 / 展开参数
来源：http://yz.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ix.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://wn.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ga.yuntaijiaju.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yl.shtwfgs.cn

Java: // 无解构
来源：http://zn.muxihuayi.cn

Go:   // 无解构
来源：http://qp.shxzukj.cn

Ruby: a, b = pair
来源：http://uo.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://tu.9csxet.cn

[C16] 函数 / 方法重载
来源：http://ik.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ei.huixiangedu.cn

PHP:  // 无重载
来源：http://sa.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jd.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://eq.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xu.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://tn.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://xc.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ob.haigaiapp.cn

================================================================================
来源：http://ce.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://es.haigaiapp.cn

================================================================================
来源：http://ta.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://re.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gu.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fg.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ct.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://st.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ip.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://it.yuexingan06.cn

Ruby: arr = [1, 2, 3]
来源：http://ff.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ls.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://su.huanxung.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://om.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wt.haigaiapp.cn

JS:   arr.push(4);
来源：http://je.yuexingan06.cn

TS:   arr.push(4);
来源：http://po.szxytkj.cn

Java: list.add(4);
来源：http://qz.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://fg.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://af.newstarts.cn

C#:   list.Add(4);
来源：http://ln.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://je.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://bv.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bb.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mq.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://by.asd995.cn

Java: list.add(0, 0);
来源：http://zr.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jp.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hf.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://xm.nszjky.cn

[D04] 删除元素
来源：http://gz.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vq.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yp.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mt.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://mp.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ae.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ji.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://va.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jd.muxihuayi.cn

[D05] 访问与修改元素
来源：http://jj.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qc.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yg.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://da.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://gx.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://me.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://us.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lo.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lk.gzmigu.cn

[D06] 数组长度
来源：http://hz.yuexingan06.cn

Py:   len(arr)
来源：http://mr.yuntaijiaju.cn

PHP:  count($arr);
来源：http://kx.colortex.cn

JS:   arr.length
来源：http://oc.asd995.cn

TS:   arr.length
来源：http://tu.chemitech.net.cn

Java: list.size();
来源：http://fz.shxzskj.cn

Go:   len(arr)
来源：http://we.nicolike.cn

Ruby: arr.length; arr.size
来源：http://ir.bookmarksfly.cn

C#:   list.Count;
来源：http://wz.newstarts.cn

[D07] 切片 / 取子数组
来源：http://qc.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jq.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://og.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://wv.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://un.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://gg.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://tz.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://zn.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://ek.chemitech.net.cn

[D08] 合并两个数组
来源：http://gc.huanxung.cn

Py:   a + b;  a.extend(b)
来源：http://sj.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://ea.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mw.shxzskj.cn

TS:   [...a, ...b];
来源：http://rp.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jf.muxihuayi.cn

Go:   append(a, b...)
来源：http://kq.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://fw.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://dv.szxytkj.cn

[D09] 排序（升序）
来源：http://op.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://jv.9csxet.cn

PHP:  sort($arr);
来源：http://ab.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ia.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ik.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rj.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ns.9csxet.cn

Ruby: arr.sort
来源：http://ef.9csxet.cn

C#:   list.Sort();
来源：http://cg.newstarts.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wb.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://se.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tm.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://su.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fi.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tr.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ao.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://if.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yx.bookmarksfly.cn

[D11] 反转数组
来源：http://lp.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sf.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://dk.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mh.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://as.shxzukj.cn

Java: Collections.reverse(list);
来源：http://rz.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://rq.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://sc.lnxyls.cn

C#:   list.Reverse();
来源：http://vj.colortex.cn

[D12] 查找元素下标
来源：http://df.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://jp.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jc.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ee.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jv.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mh.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://tu.asd995.cn

Ruby: arr.index(x)
来源：http://sp.asd995.cn

C#:   list.IndexOf(x);
来源：http://yj.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://go.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nh.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zq.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://fs.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://gj.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qm.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cc.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vi.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fx.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://wb.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ly.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qh.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://uv.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://cm.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ii.hahajie.cn

Go:   // 手写循环
来源：http://vm.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fc.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://az.lnxyls.cn

[D15] 去重
来源：http://ai.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://an.lnxyls.cn

PHP:  array_unique($arr);
来源：http://ba.newstarts.cn

JS:   [...new Set(arr)]
来源：http://bn.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://fq.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wy.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wt.jctech888.com.cn

Ruby: arr.uniq
来源：http://wn.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://up.bookmarksfly.cn

[D16] 求和与平均值
来源：http://ig.muxihuayi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hd.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hf.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ce.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fh.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jl.521024.cn

Go:   // 手写循环累加
来源：http://ec.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zs.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://hy.shxzukj.cn

[D17] 最大值与最小值
来源：http://js.colortex.cn

Py:   max(arr);  min(arr)
来源：http://so.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://ky.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vi.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://qt.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fi.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oi.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://in.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://cx.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://kz.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hp.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://td.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cr.jianghongdianzi.cn

TS:   nested.flat();
来源：http://ch.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gd.9csxet.cn

Go:   // 手写双层循环
来源：http://ph.jianghongdianzi.cn

Ruby: nested.flatten
来源：http://bl.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ed.newstarts.cn

[D19] 按字段分组
来源：http://rl.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fg.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qc.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sg.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fs.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fg.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://hn.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xy.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vc.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://ww.haigaiapp.cn

Py:   Counter(arr)
来源：http://er.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://ou.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://na.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qk.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uw.szxytkj.cn

Go:   // 手写 map[T]int
来源：http://ns.bjjhwx.cn

Ruby: arr.tally
来源：http://sb.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fd.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://pg.shxzukj.cn

Py:   x in arr
来源：http://zf.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://ap.9csxet.cn

JS:   arr.includes(x)
来源：http://cc.shxzukj.cn

TS:   arr.includes(x)
来源：http://vo.nicolike.cn

Java: list.contains(x)
来源：http://yt.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://la.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://pf.9csxet.cn

C#:   list.Contains(x)
来源：http://hk.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://dq.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xp.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sx.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nm.9csxet.cn

TS:   [...arr];
来源：http://tv.asd995.cn

Java: new ArrayList<>(list);
来源：http://lz.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xo.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://zo.muxihuayi.cn

C#:   new List<int>(list);
来源：http://ue.shtwfgs.cn

[D23] reduce 累积计算
来源：http://co.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gu.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://al.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rs.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rn.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qf.bjjhwx.cn

Go:   // 手写循环
来源：http://of.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ol.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rs.521024.cn

[D24] 字典 / Map 基本操作
来源：http://dh.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ez.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eb.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mc.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vw.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dz.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eb.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mz.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sv.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://ox.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hm.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ur.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fu.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xm.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vg.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ph.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ie.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lh.szxytkj.cn

[D26] 数组转字符串
来源：http://jk.wgjwhj.cn


<!-- 参考信息 -->