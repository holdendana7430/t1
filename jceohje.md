代发 wailian999

[C10] 变量作用域
来源：http://cp.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fu.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zw.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jb.bjjhwx.cn

TS:   同 JS
来源：http://mm.panjiajie.cn

Java: 方法内为块级作用域
来源：http://fb.asd995.cn

Go:   花括号块级作用域
来源：http://rj.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sv.haigaiapp.cn

C#:   块级作用域
来源：http://mg.shxzukj.cn

[C11] 模块导入与导出
来源：http://px.gzmigu.cn

Py:   from module import func
来源：http://xx.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jc.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pp.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wa.shxzukj.cn

Java: import java.util.List;
来源：http://dh.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gp.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://rm.yuntaijiaju.cn

C#:   using System.Text;
来源：http://sr.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://mj.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://gp.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://yw.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://ly.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://wt.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lt.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://gy.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://fw.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lp.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://mt.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hn.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nd.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mh.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qu.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ho.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://wv.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://so.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://na.huanxung.cn

[C14] 泛型函数
来源：http://gh.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hu.asd995.cn

PHP:  // 无泛型
来源：http://to.muxihuayi.cn

JS:   // 无泛型
来源：http://vf.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hy.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fm.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kg.nszjky.cn

Ruby: # 无泛型
来源：http://az.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gy.9csxet.cn

[C15] 解构 / 展开参数
来源：http://dt.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tq.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://lb.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ke.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ot.shxzukj.cn

Java: // 无解构
来源：http://oy.newstarts.cn

Go:   // 无解构
来源：http://cu.haigaiapp.cn

Ruby: a, b = pair
来源：http://kc.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://lt.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://wl.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qd.hnjuh.cn

PHP:  // 无重载
来源：http://zp.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ij.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://bx.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sa.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://ym.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://ba.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://im.haigaiapp.cn

================================================================================
来源：http://mx.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://vm.9csxet.cn

================================================================================
来源：http://cm.asd995.cn

[D01] 创建数组 / 列表
来源：http://gx.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zw.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iy.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ls.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://on.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gy.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://hl.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://zi.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://et.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://jt.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://az.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rf.colortex.cn

JS:   arr.push(4);
来源：http://da.jctech888.com.cn

TS:   arr.push(4);
来源：http://bc.szsharing.cn

Java: list.add(4);
来源：http://sk.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://la.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://tx.panjiajie.cn

C#:   list.Add(4);
来源：http://og.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://ww.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://ys.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://if.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://em.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://wv.huixiangedu.cn

Java: list.add(0, 0);
来源：http://pp.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cc.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://aj.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://dp.muxihuayi.cn

[D04] 删除元素
来源：http://cp.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jt.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ix.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fe.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://tf.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dl.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mo.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://te.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kq.colortex.cn

[D05] 访问与修改元素
来源：http://wj.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ye.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uv.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://as.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://js.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://fn.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cl.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hb.huixiangedu.cn

[D06] 数组长度
来源：http://gn.haigaiapp.cn

Py:   len(arr)
来源：http://oq.521024.cn

PHP:  count($arr);
来源：http://od.shxzukj.cn

JS:   arr.length
来源：http://jr.hahajie.cn

TS:   arr.length
来源：http://pv.colortex.cn

Java: list.size();
来源：http://im.lnxyls.cn

Go:   len(arr)
来源：http://fq.hahajie.cn

Ruby: arr.length; arr.size
来源：http://wr.nicolike.cn

C#:   list.Count;
来源：http://pv.asd995.cn

[D07] 切片 / 取子数组
来源：http://hx.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ou.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://is.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://qt.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://vr.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://xh.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://xe.gzmigu.cn

Ruby: arr[1, 3]
来源：http://dj.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://oi.panjiajie.cn

[D08] 合并两个数组
来源：http://ot.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://yp.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://cs.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pl.9csxet.cn

TS:   [...a, ...b];
来源：http://uz.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pk.newstarts.cn

Go:   append(a, b...)
来源：http://pg.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://ev.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://by.bjjhwx.cn

[D09] 排序（升序）
来源：http://yp.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://um.newstarts.cn

PHP:  sort($arr);
来源：http://yf.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://is.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hr.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fs.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wg.hnjuh.cn

Ruby: arr.sort
来源：http://qr.huixinmuqiang.cn

C#:   list.Sort();
来源：http://se.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yw.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ps.huixinmuqiang.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://od.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vr.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zz.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://et.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ov.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wy.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://of.haigaiapp.cn

[D11] 反转数组
来源：http://ds.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xb.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://dv.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wj.shxzskj.cn

TS:   [...arr].reverse();
来源：http://mj.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://ht.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://lj.nszjky.cn

Ruby: arr.reverse
来源：http://sx.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://yy.szxytkj.cn

[D12] 查找元素下标
来源：http://at.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://rx.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wk.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mu.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lw.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bp.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://kj.huixiangedu.cn

Ruby: arr.index(x)
来源：http://ch.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://kc.nszjky.cn

[D13] 过滤（保留满足条件的）
来源：http://bf.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uf.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pt.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://ig.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://hd.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ah.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sr.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sr.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uo.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://lm.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://os.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ix.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://bf.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://iv.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cv.nicolike.cn

Go:   // 手写循环
来源：http://cx.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zm.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hw.huixiangedu.cn

[D15] 去重
来源：http://rg.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fk.szxytkj.cn

PHP:  array_unique($arr);
来源：http://bs.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://is.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://hi.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wp.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yj.panjiajie.cn

Ruby: arr.uniq
来源：http://nw.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://yx.wgjwhj.cn

[D16] 求和与平均值
来源：http://yh.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://il.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ye.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pt.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cq.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jo.lnxyls.cn

Go:   // 手写循环累加
来源：http://pv.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aw.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://qi.nszjky.cn

[D17] 最大值与最小值
来源：http://zl.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://xu.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://vk.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fh.panjiajie.cn

TS:   Math.max(...arr);
来源：http://kv.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ae.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pj.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://jx.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://mf.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://lj.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ad.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://vr.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kz.colortex.cn

TS:   nested.flat();
来源：http://xa.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dg.gzmigu.cn

Go:   // 手写双层循环
来源：http://nk.muxihuayi.cn

Ruby: nested.flatten
来源：http://gr.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dq.huanxung.cn

[D19] 按字段分组
来源：http://cz.nicolike.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xg.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qv.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zf.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pl.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sg.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://qb.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tx.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dx.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://if.lnxyls.cn

Py:   Counter(arr)
来源：http://zc.newstarts.cn

PHP:  array_count_values($arr);
来源：http://gm.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uw.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ih.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yj.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://vw.panjiajie.cn

Ruby: arr.tally
来源：http://ac.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ef.newstarts.cn

[D21] 判断是否包含某元素
来源：http://ku.huixiangedu.cn

Py:   x in arr
来源：http://ox.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://wf.colortex.cn

JS:   arr.includes(x)
来源：http://au.huanxung.cn

TS:   arr.includes(x)
来源：http://wi.newstarts.cn

Java: list.contains(x)
来源：http://fn.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://el.huanxung.cn

Ruby: arr.include?(x)
来源：http://bw.9csxet.cn

C#:   list.Contains(x)
来源：http://rj.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://tz.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tv.colortex.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lw.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rt.bjjhwx.cn

TS:   [...arr];
来源：http://ql.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://vq.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fz.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://dg.jctech888.com.cn

C#:   new List<int>(list);
来源：http://ap.wgjwhj.cn

[D23] reduce 累积计算
来源：http://be.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wb.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wv.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jv.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tn.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ck.nicolike.cn

Go:   // 手写循环
来源：http://bu.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://af.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bv.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://us.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cr.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bo.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pv.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dy.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ui.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://go.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lt.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bd.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://zf.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zs.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nd.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bj.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://na.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://br.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ax.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://se.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pz.nicolike.cn

[D26] 数组转字符串
来源：http://vg.shtwfgs.cn

Py:   ", ".join(map(str, arr))
来源：http://hk.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://jo.shtwfgs.cn

JS:   arr.join(", ")
来源：http://zl.shxzskj.cn

TS:   arr.join(", ")
来源：http://ck.asd995.cn

Java: String.join(", ", list)
来源：http://pu.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://cx.hahajie.cn

Ruby: arr.join(", ")
来源：http://fw.asd995.cn

C#:   string.Join(", ", list)
来源：http://gv.newstarts.cn


<!-- 参考信息 -->