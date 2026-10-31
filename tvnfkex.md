代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vy.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vu.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vy.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ey.colortex.cn

[C10] 变量作用域
来源：http://yb.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ba.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mb.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hw.shxzukj.cn

TS:   同 JS
来源：http://jz.szsharing.cn

Java: 方法内为块级作用域
来源：http://dc.colortex.cn

Go:   花括号块级作用域
来源：http://tr.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lv.asd995.cn

C#:   块级作用域
来源：http://jr.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://cb.shxzskj.cn

Py:   from module import func
来源：http://vc.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://io.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kj.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lj.bjjhwx.cn

Java: import java.util.List;
来源：http://rl.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jj.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://du.panjiajie.cn

C#:   using System.Text;
来源：http://gs.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://ly.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://ys.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://zq.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://tx.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://gm.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rd.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://yz.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://vp.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://or.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://pv.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wo.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dl.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rh.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://id.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ah.gzmigu.cn

Go:   func add(a, b int) int
来源：http://fj.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eu.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lj.hnjuh.cn

[C14] 泛型函数
来源：http://qn.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ob.chemitech.net.cn

PHP:  // 无泛型
来源：http://vr.nicolike.cn

JS:   // 无泛型
来源：http://py.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vw.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lt.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yj.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://lr.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fn.521024.cn

[C15] 解构 / 展开参数
来源：http://ud.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xf.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://cb.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ay.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rc.chemitech.net.cn

Java: // 无解构
来源：http://rr.shtwfgs.cn

Go:   // 无解构
来源：http://sy.panjiajie.cn

Ruby: a, b = pair
来源：http://pq.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://th.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://nn.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xp.colortex.cn

PHP:  // 无重载
来源：http://ee.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bt.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://lq.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://op.muxihuayi.cn

Go:   // 无重载：用不同函数名
来源：http://do.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://zo.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jy.shtwfgs.cn

================================================================================
来源：http://zy.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://nh.jianghongdianzi.cn

================================================================================
来源：http://gw.521024.cn

[D01] 创建数组 / 列表
来源：http://gw.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jq.shtwfgs.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iq.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cx.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ch.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vm.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://hq.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://gz.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iy.9csxet.cn

[D02] 追加元素到末尾
来源：http://bs.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xe.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://um.bookmarksfly.cn

JS:   arr.push(4);
来源：http://hz.gzmigu.cn

TS:   arr.push(4);
来源：http://om.521024.cn

Java: list.add(4);
来源：http://qo.colortex.cn

Go:   arr = append(arr, 4)
来源：http://ks.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://fj.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://ss.huanxung.cn

[D03] 在指定位置插入元素
来源：http://fv.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://ue.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ox.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ei.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://rw.newstarts.cn

Java: list.add(0, 0);
来源：http://yb.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rg.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mu.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://qa.jctech888.com.cn

[D04] 删除元素
来源：http://ka.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pp.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ln.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ij.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://mh.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://id.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fa.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pr.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bc.shxzskj.cn

[D05] 访问与修改元素
来源：http://og.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hy.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rh.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jg.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://ux.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://wj.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://rs.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tg.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ce.jianghongdianzi.cn

[D06] 数组长度
来源：http://es.bjjhwx.cn

Py:   len(arr)
来源：http://rd.szxytkj.cn

PHP:  count($arr);
来源：http://of.szxytkj.cn

JS:   arr.length
来源：http://us.shxzskj.cn

TS:   arr.length
来源：http://tc.gzmigu.cn

Java: list.size();
来源：http://pf.gzmigu.cn

Go:   len(arr)
来源：http://gj.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://zs.asd995.cn

C#:   list.Count;
来源：http://eq.asd995.cn

[D07] 切片 / 取子数组
来源：http://vy.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wx.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hj.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://os.colortex.cn

TS:   arr.slice(1, 4);
来源：http://wj.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://oa.bookmarksfly.cn

Go:   arr[1:4]
来源：http://gh.szxytkj.cn

Ruby: arr[1, 3]
来源：http://qd.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://ov.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://ck.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://kb.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://xj.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lw.lnxyls.cn

TS:   [...a, ...b];
来源：http://ar.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ip.jctech888.com.cn

Go:   append(a, b...)
来源：http://ti.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://nv.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://nb.bjjhwx.cn

[D09] 排序（升序）
来源：http://zx.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://qu.9csxet.cn

PHP:  sort($arr);
来源：http://te.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://js.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ke.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mn.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://um.yuntaijiaju.cn

Ruby: arr.sort
来源：http://yw.wgjwhj.cn

C#:   list.Sort();
来源：http://rj.newstarts.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ep.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iw.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://er.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gm.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yw.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ta.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ho.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qj.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kq.huixiangedu.cn

[D11] 反转数组
来源：http://qe.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://io.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://yz.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qk.szxytkj.cn

TS:   [...arr].reverse();
来源：http://he.szsharing.cn

Java: Collections.reverse(list);
来源：http://pg.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://pi.szsharing.cn

Ruby: arr.reverse
来源：http://qw.jctech888.com.cn

C#:   list.Reverse();
来源：http://nc.muxihuayi.cn

[D12] 查找元素下标
来源：http://zj.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://my.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jt.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sb.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oo.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jj.colortex.cn

Go:   slices.Index(arr, x)
来源：http://bx.szxytkj.cn

Ruby: arr.index(x)
来源：http://oa.newstarts.cn

C#:   list.IndexOf(x);
来源：http://kf.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://mn.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ew.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ux.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://qz.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://mi.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ap.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://on.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://au.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yr.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://zy.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hm.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://df.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://jt.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://va.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yp.panjiajie.cn

Go:   // 手写循环
来源：http://ex.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bl.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pp.shxzskj.cn

[D15] 去重
来源：http://dp.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pk.shxzukj.cn

PHP:  array_unique($arr);
来源：http://mz.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://mh.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://yy.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vp.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yj.wgjwhj.cn

Ruby: arr.uniq
来源：http://dq.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://je.bjjhwx.cn

[D16] 求和与平均值
来源：http://vo.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vv.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zl.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://be.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xj.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jh.hnjuh.cn

Go:   // 手写循环累加
来源：http://xv.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hi.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://tk.szxytkj.cn

[D17] 最大值与最小值
来源：http://fb.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://fe.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://wv.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iu.panjiajie.cn

TS:   Math.max(...arr);
来源：http://ty.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cn.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://or.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://cv.521024.cn

C#:   list.Max();  list.Min()
来源：http://fi.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://ah.muxihuayi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zb.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://vu.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gf.hahajie.cn

TS:   nested.flat();
来源：http://do.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zg.panjiajie.cn

Go:   // 手写双层循环
来源：http://sz.muxihuayi.cn

Ruby: nested.flatten
来源：http://br.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gg.huixiangedu.cn

[D19] 按字段分组
来源：http://oz.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oj.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kp.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ub.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ey.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wt.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://fk.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rm.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ha.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://cb.gzmigu.cn

Py:   Counter(arr)
来源：http://rw.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://xb.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tq.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mv.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rz.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://jj.szxytkj.cn

Ruby: arr.tally
来源：http://yt.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pq.hahajie.cn

[D21] 判断是否包含某元素
来源：http://gw.huixiangedu.cn

Py:   x in arr
来源：http://by.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://cn.hnjuh.cn

JS:   arr.includes(x)
来源：http://yc.bjjhwx.cn

TS:   arr.includes(x)
来源：http://ao.nicolike.cn

Java: list.contains(x)
来源：http://rl.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://vr.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://nx.jctech888.com.cn

C#:   list.Contains(x)
来源：http://vj.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://gt.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ia.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xt.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kr.newstarts.cn

TS:   [...arr];
来源：http://xp.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://ng.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fn.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://hy.nszjky.cn

C#:   new List<int>(list);
来源：http://lk.gzmigu.cn

[D23] reduce 累积计算
来源：http://yj.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://al.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xg.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tb.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qh.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vl.bookmarksfly.cn

Go:   // 手写循环
来源：http://dq.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ra.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ic.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://me.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://aw.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ly.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aw.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://my.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tq.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ti.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tm.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ae.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://vd.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cf.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bi.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://di.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rc.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://am.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ol.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zk.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ba.chemitech.net.cn

[D26] 数组转字符串
来源：http://iy.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://kz.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://wh.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://hl.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://sd.szsharing.cn


<!-- 参考信息 -->