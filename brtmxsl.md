代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hh.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ba.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://od.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://us.huixiangedu.cn

[C10] 变量作用域
来源：http://gy.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mc.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jt.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zx.yuntaijiaju.cn

TS:   同 JS
来源：http://tl.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://wp.shtwfgs.cn

Go:   花括号块级作用域
来源：http://sy.huixiangedu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oc.gzmigu.cn

C#:   块级作用域
来源：http://nt.jctech888.com.cn

[C11] 模块导入与导出
来源：http://rw.lnxyls.cn

Py:   from module import func
来源：http://mx.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bd.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ud.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kt.jctech888.com.cn

Java: import java.util.List;
来源：http://nj.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://io.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://kw.shxzukj.cn

C#:   using System.Text;
来源：http://wc.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://yi.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://on.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://xi.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://hk.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://et.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://od.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://rw.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://zb.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tq.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://ju.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vj.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yy.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qg.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://za.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ut.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://yg.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://no.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vs.nicolike.cn

[C14] 泛型函数
来源：http://mc.asd995.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://so.shtwfgs.cn

PHP:  // 无泛型
来源：http://se.bookmarksfly.cn

JS:   // 无泛型
来源：http://sa.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cd.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hd.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pp.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://fr.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ej.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://re.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qk.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://oa.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pa.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lh.gzmigu.cn

Java: // 无解构
来源：http://wp.huixinmuqiang.cn

Go:   // 无解构
来源：http://un.jctech888.com.cn

Ruby: a, b = pair
来源：http://zw.hahajie.cn

C#:   var (a, b) = pair;
来源：http://lr.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://kn.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dp.bookmarksfly.cn

PHP:  // 无重载
来源：http://pq.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tn.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://eh.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://id.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://kc.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://vc.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rh.nicolike.cn

================================================================================
来源：http://sd.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://ar.bookmarksfly.cn

================================================================================
来源：http://lr.colortex.cn

[D01] 创建数组 / 列表
来源：http://ai.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oh.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yk.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://be.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ck.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lc.shtwfgs.cn

Go:   arr := []int{1, 2, 3}
来源：http://wd.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://yy.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mn.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://lb.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xz.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wj.nicolike.cn

JS:   arr.push(4);
来源：http://on.yuexingan06.cn

TS:   arr.push(4);
来源：http://jv.bookmarksfly.cn

Java: list.add(4);
来源：http://lj.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://rg.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://gv.huanxung.cn

C#:   list.Add(4);
来源：http://pe.huanxung.cn

[D03] 在指定位置插入元素
来源：http://hl.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://fu.lnxyls.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gt.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xx.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://xg.hahajie.cn

Java: list.add(0, 0);
来源：http://to.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yy.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ff.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://vw.shxzukj.cn

[D04] 删除元素
来源：http://rm.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ho.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zo.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://us.jctech888.com.cn

TS:   arr.splice(0, 1);
来源：http://lf.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fm.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gr.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rc.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oy.nicolike.cn

[D05] 访问与修改元素
来源：http://ls.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ta.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://km.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vd.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://ud.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://av.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://cz.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ug.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pm.yuexingan06.cn

[D06] 数组长度
来源：http://ev.huanxung.cn

Py:   len(arr)
来源：http://ow.huanxung.cn

PHP:  count($arr);
来源：http://zr.colortex.cn

JS:   arr.length
来源：http://mt.muxihuayi.cn

TS:   arr.length
来源：http://ym.panjiajie.cn

Java: list.size();
来源：http://ca.szxytkj.cn

Go:   len(arr)
来源：http://rk.asd995.cn

Ruby: arr.length; arr.size
来源：http://rc.muxihuayi.cn

C#:   list.Count;
来源：http://sx.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://fj.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://an.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yf.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://ci.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://pa.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://zs.asd995.cn

Go:   arr[1:4]
来源：http://ld.nicolike.cn

Ruby: arr[1, 3]
来源：http://kd.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://sh.bookmarksfly.cn

[D08] 合并两个数组
来源：http://vq.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://uv.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://pr.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ou.lnxyls.cn

TS:   [...a, ...b];
来源：http://fg.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fl.shxzskj.cn

Go:   append(a, b...)
来源：http://me.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://lf.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://ec.chemitech.net.cn

[D09] 排序（升序）
来源：http://uk.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://yv.asd995.cn

PHP:  sort($arr);
来源：http://aa.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ud.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://aj.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xg.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kd.521024.cn

Ruby: arr.sort
来源：http://xf.yuntaijiaju.cn

C#:   list.Sort();
来源：http://wy.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vy.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nb.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cr.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hx.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wn.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zr.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nh.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ek.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cv.asd995.cn

[D11] 反转数组
来源：http://cb.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ug.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://wm.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tu.huanxung.cn

TS:   [...arr].reverse();
来源：http://pi.asd995.cn

Java: Collections.reverse(list);
来源：http://ul.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://sa.newstarts.cn

Ruby: arr.reverse
来源：http://nx.haigaiapp.cn

C#:   list.Reverse();
来源：http://ij.huanxung.cn

[D12] 查找元素下标
来源：http://un.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://gv.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yv.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uy.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bg.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pc.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://wj.szxytkj.cn

Ruby: arr.index(x)
来源：http://an.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://mi.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://ta.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yv.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ef.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://qt.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://it.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ae.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xi.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xr.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cw.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://rj.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xw.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eq.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://dx.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://hc.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://js.jianghongdianzi.cn

Go:   // 手写循环
来源：http://qu.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yc.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jf.asd995.cn

[D15] 去重
来源：http://hu.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kc.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://ji.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://yj.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://hr.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lp.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vs.shxzskj.cn

Ruby: arr.uniq
来源：http://cc.colortex.cn

C#:   list.Distinct().ToList()
来源：http://xy.newstarts.cn

[D16] 求和与平均值
来源：http://gf.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xq.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dv.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kk.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lg.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wy.shxzskj.cn

Go:   // 手写循环累加
来源：http://zv.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mv.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://gi.lnxyls.cn

[D17] 最大值与最小值
来源：http://on.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://yn.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://qz.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qc.asd995.cn

TS:   Math.max(...arr);
来源：http://yn.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kr.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ll.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://ll.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://bq.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://ah.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qi.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://tl.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cg.bjjhwx.cn

TS:   nested.flat();
来源：http://pp.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://un.szsharing.cn

Go:   // 手写双层循环
来源：http://xu.huanxung.cn

Ruby: nested.flatten
来源：http://ts.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hh.chemitech.net.cn

[D19] 按字段分组
来源：http://ft.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ua.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ig.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fd.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://be.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bm.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://so.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kv.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zk.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://hi.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://vs.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://rf.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pk.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cu.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://go.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://zs.lnxyls.cn

Ruby: arr.tally
来源：http://ut.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lm.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://lc.jctech888.com.cn

Py:   x in arr
来源：http://eg.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://em.shxzukj.cn

JS:   arr.includes(x)
来源：http://lf.shxzskj.cn

TS:   arr.includes(x)
来源：http://ww.huixiangedu.cn

Java: list.contains(x)
来源：http://gs.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://ww.gzmigu.cn

Ruby: arr.include?(x)
来源：http://ae.huixiangedu.cn

C#:   list.Contains(x)
来源：http://vv.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://ny.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nh.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dj.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iy.asd995.cn

TS:   [...arr];
来源：http://ew.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://ii.chemitech.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sg.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://ky.hahajie.cn

C#:   new List<int>(list);
来源：http://wc.panjiajie.cn

[D23] reduce 累积计算
来源：http://zv.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://th.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vg.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://if.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fe.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fx.muxihuayi.cn

Go:   // 手写循环
来源：http://ez.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cm.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tl.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://vr.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ed.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ui.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tj.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kx.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ah.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ad.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tl.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vj.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://gk.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tw.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pz.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qj.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lc.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qt.huanxung.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gl.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gg.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ek.jctech888.com.cn

[D26] 数组转字符串
来源：http://ey.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://kr.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://sq.nicolike.cn

JS:   arr.join(", ")
来源：http://pq.panjiajie.cn

TS:   arr.join(", ")
来源：http://to.bjjhwx.cn


<!-- 参考信息 -->