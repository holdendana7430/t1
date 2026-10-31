代发 wailian999

[C10] 变量作用域
来源：http://ol.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jj.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nx.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rs.521024.cn

TS:   同 JS
来源：http://yr.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://ma.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://qt.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ez.shtwfgs.cn

C#:   块级作用域
来源：http://xb.hahajie.cn

[C11] 模块导入与导出
来源：http://fk.chemitech.net.cn

Py:   from module import func
来源：http://re.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ni.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ib.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fl.gzmigu.cn

Java: import java.util.List;
来源：http://cf.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iv.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://tb.9csxet.cn

C#:   using System.Text;
来源：http://jr.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://if.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://pf.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://py.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://sr.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://cw.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://di.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://hw.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://yu.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hf.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://yx.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gd.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tv.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ka.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mj.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://va.szsharing.cn

Go:   func add(a, b int) int
来源：http://ir.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kt.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zk.jctech888.com.cn

[C14] 泛型函数
来源：http://vv.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lz.yuexingan06.cn

PHP:  // 无泛型
来源：http://zc.9csxet.cn

JS:   // 无泛型
来源：http://yg.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://db.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kn.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nm.nicolike.cn

Ruby: # 无泛型
来源：http://xl.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lg.9csxet.cn

[C15] 解构 / 展开参数
来源：http://fa.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iy.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://iz.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xh.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xn.shxzukj.cn

Java: // 无解构
来源：http://ev.lnxyls.cn

Go:   // 无解构
来源：http://xv.colortex.cn

Ruby: a, b = pair
来源：http://hy.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://gw.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://um.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ke.chemitech.net.cn

PHP:  // 无重载
来源：http://lh.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://re.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://sf.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gw.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://sw.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://gk.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fd.nicolike.cn

================================================================================
来源：http://fo.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://js.haigaiapp.cn

================================================================================
来源：http://dm.huanxung.cn

[D01] 创建数组 / 列表
来源：http://wq.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wo.shtwfgs.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ct.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://me.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wf.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://co.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://cw.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://ux.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kc.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://qc.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fs.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hx.shxzskj.cn

JS:   arr.push(4);
来源：http://ec.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://ft.nszjky.cn

Java: list.add(4);
来源：http://uf.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://wi.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ix.shxzukj.cn

C#:   list.Add(4);
来源：http://go.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://ba.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://bn.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pr.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ek.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://je.asd995.cn

Java: list.add(0, 0);
来源：http://mr.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pe.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ep.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://sr.asd995.cn

[D04] 删除元素
来源：http://fe.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mc.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zd.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nb.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://tw.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iv.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tz.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vw.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ci.nszjky.cn

[D05] 访问与修改元素
来源：http://an.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eh.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ax.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ou.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://hi.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://yz.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://tb.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pz.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pz.nicolike.cn

[D06] 数组长度
来源：http://vl.yuntaijiaju.cn

Py:   len(arr)
来源：http://gh.shxzukj.cn

PHP:  count($arr);
来源：http://wr.shxzskj.cn

JS:   arr.length
来源：http://qt.hnjuh.cn

TS:   arr.length
来源：http://cp.gzmigu.cn

Java: list.size();
来源：http://xn.bjjhwx.cn

Go:   len(arr)
来源：http://bi.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://hg.chemitech.net.cn

C#:   list.Count;
来源：http://ty.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://qv.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tc.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cu.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://ze.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://ne.9csxet.cn

Java: list.subList(1, 4);
来源：http://hb.huixiangedu.cn

Go:   arr[1:4]
来源：http://kr.huanxung.cn

Ruby: arr[1, 3]
来源：http://yu.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://mi.asd995.cn

[D08] 合并两个数组
来源：http://ft.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://ik.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://re.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nw.shxzukj.cn

TS:   [...a, ...b];
来源：http://oe.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sd.szxytkj.cn

Go:   append(a, b...)
来源：http://va.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://ny.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://qm.wgjwhj.cn

[D09] 排序（升序）
来源：http://lj.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://br.haigaiapp.cn

PHP:  sort($arr);
来源：http://eq.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bj.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://il.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ta.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xl.bjjhwx.cn

Ruby: arr.sort
来源：http://sy.asd995.cn

C#:   list.Sort();
来源：http://uk.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tf.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ux.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://st.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fc.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ua.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jo.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ws.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zl.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lj.521024.cn

[D11] 反转数组
来源：http://ck.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://eg.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://wu.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ji.panjiajie.cn

TS:   [...arr].reverse();
来源：http://ch.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://ls.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://dk.nszjky.cn

Ruby: arr.reverse
来源：http://to.lnxyls.cn

C#:   list.Reverse();
来源：http://pt.szxytkj.cn

[D12] 查找元素下标
来源：http://gy.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://ya.newstarts.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://up.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://md.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bp.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cj.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://sd.shxzukj.cn

Ruby: arr.index(x)
来源：http://jq.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://nr.nszjky.cn

[D13] 过滤（保留满足条件的）
来源：http://nj.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wk.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ls.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://uf.szsharing.cn

TS:   arr.filter(x => x > 3)
来源：http://kp.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ri.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rk.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vl.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vy.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://pw.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lc.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wo.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://uf.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://vi.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yj.yuexingan06.cn

Go:   // 手写循环
来源：http://li.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mz.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bj.shxzskj.cn

[D15] 去重
来源：http://ev.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bp.521024.cn

PHP:  array_unique($arr);
来源：http://mq.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://gk.nszjky.cn

TS:   [...new Set(arr)]
来源：http://cs.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lf.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uo.jctech888.com.cn

Ruby: arr.uniq
来源：http://ca.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://yd.521024.cn

[D16] 求和与平均值
来源：http://fo.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lg.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qv.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oh.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vu.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gn.chemitech.net.cn

Go:   // 手写循环累加
来源：http://ek.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lg.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://cf.521024.cn

[D17] 最大值与最小值
来源：http://jx.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://cq.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://zi.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jh.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://mj.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tf.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://io.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://ry.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://fm.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://bh.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vp.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://ws.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dr.wgjwhj.cn

TS:   nested.flat();
来源：http://qn.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://go.gzmigu.cn

Go:   // 手写双层循环
来源：http://cp.hnjuh.cn

Ruby: nested.flatten
来源：http://yb.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vs.bookmarksfly.cn

[D19] 按字段分组
来源：http://ky.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jr.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qq.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lm.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zl.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bx.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://lm.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cc.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zi.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://fl.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://vs.nicolike.cn

PHP:  array_count_values($arr);
来源：http://xa.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jt.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ty.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ni.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://lg.yuntaijiaju.cn

Ruby: arr.tally
来源：http://gy.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tf.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://wu.chemitech.net.cn

Py:   x in arr
来源：http://jd.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://ug.nicolike.cn

JS:   arr.includes(x)
来源：http://jy.huanxung.cn

TS:   arr.includes(x)
来源：http://sy.gzmigu.cn

Java: list.contains(x)
来源：http://le.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://mw.521024.cn

Ruby: arr.include?(x)
来源：http://ub.szsharing.cn

C#:   list.Contains(x)
来源：http://gf.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://hx.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sx.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qk.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://os.shxzukj.cn

TS:   [...arr];
来源：http://tz.asd995.cn

Java: new ArrayList<>(list);
来源：http://je.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dm.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://zm.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://lj.huanxung.cn

[D23] reduce 累积计算
来源：http://ee.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qw.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://os.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xe.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zk.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ch.colortex.cn

Go:   // 手写循环
来源：http://te.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rl.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sd.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://bc.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hv.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yp.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ze.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cj.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://go.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ef.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pt.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sd.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://ab.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ey.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ne.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wa.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://et.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ab.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gr.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sr.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nm.jctech888.com.cn

[D26] 数组转字符串
来源：http://md.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://xy.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://tq.huanxung.cn

JS:   arr.join(", ")
来源：http://ug.gzmigu.cn

TS:   arr.join(", ")
来源：http://sw.lnxyls.cn

Java: String.join(", ", list)
来源：http://qs.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://pw.panjiajie.cn

Ruby: arr.join(", ")
来源：http://bg.asd995.cn

C#:   string.Join(", ", list)
来源：http://ha.jianghongdianzi.cn


<!-- 参考信息 -->