代发 wailian999

[C10] 变量作用域
来源：http://if.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zc.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sg.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ys.bookmarksfly.cn

TS:   同 JS
来源：http://wi.9csxet.cn

Java: 方法内为块级作用域
来源：http://my.shtwfgs.cn

Go:   花括号块级作用域
来源：http://ce.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uf.gzmigu.cn

C#:   块级作用域
来源：http://hk.yuexingan06.cn

[C11] 模块导入与导出
来源：http://bb.hahajie.cn

Py:   from module import func
来源：http://ik.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zx.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jw.9csxet.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jw.chemitech.net.cn

Java: import java.util.List;
来源：http://ol.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zb.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://gb.gzmigu.cn

C#:   using System.Text;
来源：http://jq.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://mo.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://il.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://nt.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://bn.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://ou.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zb.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://tm.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://so.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ch.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://rn.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fh.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iw.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mv.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yf.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yj.newstarts.cn

Go:   func add(a, b int) int
来源：http://sc.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://em.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uk.huanxung.cn

[C14] 泛型函数
来源：http://kc.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zb.shtwfgs.cn

PHP:  // 无泛型
来源：http://uq.bookmarksfly.cn

JS:   // 无泛型
来源：http://ne.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rt.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hb.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mv.newstarts.cn

Ruby: # 无泛型
来源：http://ev.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cg.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://gk.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vt.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://eu.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ty.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nz.lnxyls.cn

Java: // 无解构
来源：http://de.nicolike.cn

Go:   // 无解构
来源：http://bk.521024.cn

Ruby: a, b = pair
来源：http://el.nszjky.cn

C#:   var (a, b) = pair;
来源：http://jn.hahajie.cn

[C16] 函数 / 方法重载
来源：http://ny.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sr.wgjwhj.cn

PHP:  // 无重载
来源：http://tj.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xe.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://dq.panjiajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cs.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://wo.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://ue.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://av.hnjuh.cn

================================================================================
来源：http://nz.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://xz.huanxung.cn

================================================================================
来源：http://pr.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://lv.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://is.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lj.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hd.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bw.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jg.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://gh.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://dm.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://op.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://fb.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wg.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gh.bookmarksfly.cn

JS:   arr.push(4);
来源：http://gr.nszjky.cn

TS:   arr.push(4);
来源：http://sb.hahajie.cn

Java: list.add(4);
来源：http://sn.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://cb.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://kc.hahajie.cn

C#:   list.Add(4);
来源：http://nb.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://ws.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://yv.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hf.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hq.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://is.hahajie.cn

Java: list.add(0, 0);
来源：http://ft.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ur.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://aj.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://hl.szsharing.cn

[D04] 删除元素
来源：http://et.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gt.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zg.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ka.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://yv.bookmarksfly.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ow.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qk.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ga.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xq.colortex.cn

[D05] 访问与修改元素
来源：http://vp.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ln.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ii.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cp.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://gf.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://ew.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://rk.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bq.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xc.yuntaijiaju.cn

[D06] 数组长度
来源：http://xw.521024.cn

Py:   len(arr)
来源：http://ct.colortex.cn

PHP:  count($arr);
来源：http://ft.huixiangedu.cn

JS:   arr.length
来源：http://hj.shtwfgs.cn

TS:   arr.length
来源：http://op.colortex.cn

Java: list.size();
来源：http://qj.chemitech.net.cn

Go:   len(arr)
来源：http://ft.521024.cn

Ruby: arr.length; arr.size
来源：http://ko.wgjwhj.cn

C#:   list.Count;
来源：http://gq.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://yd.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://db.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kb.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://wk.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://xm.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://mz.chemitech.net.cn

Go:   arr[1:4]
来源：http://ea.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://ca.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://tn.lnxyls.cn

[D08] 合并两个数组
来源：http://ic.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://na.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://mp.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qh.colortex.cn

TS:   [...a, ...b];
来源：http://yz.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kl.bookmarksfly.cn

Go:   append(a, b...)
来源：http://ew.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://bd.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://hl.shtwfgs.cn

[D09] 排序（升序）
来源：http://mx.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://tm.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://ni.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://or.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tl.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ob.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tk.jctech888.com.cn

Ruby: arr.sort
来源：http://mt.huixiangedu.cn

C#:   list.Sort();
来源：http://rk.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nf.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sn.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ks.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tr.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ma.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ku.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qk.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zk.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jq.asd995.cn

[D11] 反转数组
来源：http://mj.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ox.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://wh.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ky.9csxet.cn

TS:   [...arr].reverse();
来源：http://lg.521024.cn

Java: Collections.reverse(list);
来源：http://xm.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://up.bjjhwx.cn

Ruby: arr.reverse
来源：http://tx.yuexingan06.cn

C#:   list.Reverse();
来源：http://si.bjjhwx.cn

[D12] 查找元素下标
来源：http://cz.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://al.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mn.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ug.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nq.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fm.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://fw.bjjhwx.cn

Ruby: arr.index(x)
来源：http://me.9csxet.cn

C#:   list.IndexOf(x);
来源：http://hv.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://zt.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pl.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xf.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://ir.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://jb.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qk.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jy.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fs.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pm.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://nu.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://em.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pf.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://oj.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://hw.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://af.nszjky.cn

Go:   // 手写循环
来源：http://ua.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ya.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://le.panjiajie.cn

[D15] 去重
来源：http://qp.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ca.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://df.nszjky.cn

JS:   [...new Set(arr)]
来源：http://gq.nicolike.cn

TS:   [...new Set(arr)]
来源：http://tt.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lt.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mz.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://vl.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://yp.gzmigu.cn

[D16] 求和与平均值
来源：http://cx.chemitech.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ur.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://od.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://of.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jc.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cu.shxzskj.cn

Go:   // 手写循环累加
来源：http://qq.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wj.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://cw.yuexingan06.cn

[D17] 最大值与最小值
来源：http://bo.colortex.cn

Py:   max(arr);  min(arr)
来源：http://uw.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://sc.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oj.szsharing.cn

TS:   Math.max(...arr);
来源：http://oc.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xj.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pa.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://to.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://me.haigaiapp.cn

[D18] 扁平化嵌套数组
来源：http://rz.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wi.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://iy.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ie.huixinmuqiang.cn

TS:   nested.flat();
来源：http://bl.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cu.nszjky.cn

Go:   // 手写双层循环
来源：http://pb.colortex.cn

Ruby: nested.flatten
来源：http://hf.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gl.521024.cn

[D19] 按字段分组
来源：http://zo.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kz.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zs.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rj.colortex.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ep.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://id.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://id.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sx.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ue.muxihuayi.cn

[D20] 统计每个元素出现次数
来源：http://td.jctech888.com.cn

Py:   Counter(arr)
来源：http://qx.huanxung.cn

PHP:  array_count_values($arr);
来源：http://ho.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ce.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yp.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ic.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://qx.panjiajie.cn

Ruby: arr.tally
来源：http://zx.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hn.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://pg.wgjwhj.cn

Py:   x in arr
来源：http://hv.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://vj.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://ym.haigaiapp.cn

TS:   arr.includes(x)
来源：http://hp.jctech888.com.cn

Java: list.contains(x)
来源：http://ug.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://kc.panjiajie.cn

Ruby: arr.include?(x)
来源：http://sl.521024.cn

C#:   list.Contains(x)
来源：http://sd.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://bz.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tf.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fs.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nh.9csxet.cn

TS:   [...arr];
来源：http://zf.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://gn.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ol.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://kd.nicolike.cn

C#:   new List<int>(list);
来源：http://jj.asd995.cn

[D23] reduce 累积计算
来源：http://hy.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qs.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ke.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pw.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xi.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://iu.nicolike.cn

Go:   // 手写循环
来源：http://sn.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nw.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dw.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://qu.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ft.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wx.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bg.colortex.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mx.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lg.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zc.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://as.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fa.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://uq.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xu.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kk.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ci.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rk.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sk.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xp.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kx.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lz.haigaiapp.cn

[D26] 数组转字符串
来源：http://kr.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://ta.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://rs.chemitech.net.cn

JS:   arr.join(", ")
来源：http://at.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://zv.huixiangedu.cn

Java: String.join(", ", list)
来源：http://ue.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://za.gzmigu.cn

Ruby: arr.join(", ")
来源：http://gr.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://ne.lnxyls.cn


<!-- 参考信息 -->