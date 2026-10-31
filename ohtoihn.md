代发 wailian999

[C10] 变量作用域
来源：http://ak.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hp.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kv.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dp.muxihuayi.cn

TS:   同 JS
来源：http://th.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://ub.hahajie.cn

Go:   花括号块级作用域
来源：http://gw.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pc.chemitech.net.cn

C#:   块级作用域
来源：http://xo.huanxung.cn

[C11] 模块导入与导出
来源：http://za.szxytkj.cn

Py:   from module import func
来源：http://ut.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jn.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mc.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://aq.lnxyls.cn

Java: import java.util.List;
来源：http://gt.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://va.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://kn.colortex.cn

C#:   using System.Text;
来源：http://gf.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://nn.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://kt.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://ap.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://ma.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://tu.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rq.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://ry.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://og.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yn.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://wh.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vj.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://is.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xc.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bq.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sh.szxytkj.cn

Go:   func add(a, b int) int
来源：http://ba.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xl.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sn.colortex.cn

[C14] 泛型函数
来源：http://jz.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://we.huixiangedu.cn

PHP:  // 无泛型
来源：http://tb.jianghongdianzi.cn

JS:   // 无泛型
来源：http://oe.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mz.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://al.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oj.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://uk.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xg.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://cz.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nw.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://vk.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yq.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nr.asd995.cn

Java: // 无解构
来源：http://sq.bookmarksfly.cn

Go:   // 无解构
来源：http://jh.wgjwhj.cn

Ruby: a, b = pair
来源：http://pl.hahajie.cn

C#:   var (a, b) = pair;
来源：http://zb.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://fz.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rc.asd995.cn

PHP:  // 无重载
来源：http://nb.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uz.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://sf.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ub.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://if.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://di.colortex.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yg.yuexingan06.cn

================================================================================
来源：http://fd.asd995.cn

D. 数组 / 列表 / 集合
来源：http://iz.colortex.cn

================================================================================
来源：http://vi.521024.cn

[D01] 创建数组 / 列表
来源：http://fq.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jg.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ot.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lb.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hb.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uj.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://bc.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://tn.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ii.hnjuh.cn

[D02] 追加元素到末尾
来源：http://bc.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xe.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hj.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://ef.9csxet.cn

TS:   arr.push(4);
来源：http://my.bjjhwx.cn

Java: list.add(4);
来源：http://xk.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://ww.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://tb.yuexingan06.cn

C#:   list.Add(4);
来源：http://ye.9csxet.cn

[D03] 在指定位置插入元素
来源：http://st.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://vo.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cm.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ss.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ho.colortex.cn

Java: list.add(0, 0);
来源：http://nc.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sl.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kn.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://fv.hahajie.cn

[D04] 删除元素
来源：http://cy.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://si.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dd.szsharing.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vz.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://qg.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mg.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wn.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dq.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fn.huixiangedu.cn

[D05] 访问与修改元素
来源：http://ff.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zk.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ox.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wv.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://po.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://rf.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://ms.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tw.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jj.jianghongdianzi.cn

[D06] 数组长度
来源：http://nx.9csxet.cn

Py:   len(arr)
来源：http://mu.yuexingan06.cn

PHP:  count($arr);
来源：http://qb.shxzukj.cn

JS:   arr.length
来源：http://th.haigaiapp.cn

TS:   arr.length
来源：http://zo.9csxet.cn

Java: list.size();
来源：http://fg.wgjwhj.cn

Go:   len(arr)
来源：http://kw.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://mo.huanxung.cn

C#:   list.Count;
来源：http://qs.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://hh.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ys.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pt.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://yr.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://wv.asd995.cn

Java: list.subList(1, 4);
来源：http://ks.nszjky.cn

Go:   arr[1:4]
来源：http://qa.hnjuh.cn

Ruby: arr[1, 3]
来源：http://jf.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://nw.gzmigu.cn

[D08] 合并两个数组
来源：http://cj.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://bc.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://ry.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oq.newstarts.cn

TS:   [...a, ...b];
来源：http://pi.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://li.521024.cn

Go:   append(a, b...)
来源：http://xw.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://tz.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://kc.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://ig.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://nq.shxzukj.cn

PHP:  sort($arr);
来源：http://rc.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mt.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kx.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kd.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kq.newstarts.cn

Ruby: arr.sort
来源：http://uy.bookmarksfly.cn

C#:   list.Sort();
来源：http://wc.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ow.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fx.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kv.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pg.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tn.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ye.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vw.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://is.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ws.jctech888.com.cn

[D11] 反转数组
来源：http://dw.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hu.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://py.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dk.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://mo.9csxet.cn

Java: Collections.reverse(list);
来源：http://ie.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://xx.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://jn.wgjwhj.cn

C#:   list.Reverse();
来源：http://mt.gzmigu.cn

[D12] 查找元素下标
来源：http://kh.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://mv.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rt.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eq.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pc.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ea.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://ar.hahajie.cn

Ruby: arr.index(x)
来源：http://dv.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://nm.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://an.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zg.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qf.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://eu.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://ov.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ia.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xd.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zh.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dw.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://tl.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ln.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yc.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://uq.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://up.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ti.asd995.cn

Go:   // 手写循环
来源：http://md.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lo.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pn.yuexingan06.cn

[D15] 去重
来源：http://ns.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kg.asd995.cn

PHP:  array_unique($arr);
来源：http://hd.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://dn.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://ay.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://br.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sg.panjiajie.cn

Ruby: arr.uniq
来源：http://gq.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://mr.lnxyls.cn

[D16] 求和与平均值
来源：http://bt.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wd.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ed.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fq.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dd.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hx.szxytkj.cn

Go:   // 手写循环累加
来源：http://bh.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ht.521024.cn

C#:   list.Sum();  list.Average()
来源：http://zy.bjjhwx.cn

[D17] 最大值与最小值
来源：http://pq.asd995.cn

Py:   max(arr);  min(arr)
来源：http://bw.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://hx.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nb.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://rw.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nk.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fn.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://fr.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://kc.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://xf.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bn.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://uc.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ex.gzmigu.cn

TS:   nested.flat();
来源：http://ru.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ap.newstarts.cn

Go:   // 手写双层循环
来源：http://nh.521024.cn

Ruby: nested.flatten
来源：http://sj.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ik.szsharing.cn

[D19] 按字段分组
来源：http://bq.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uf.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lw.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wl.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://in.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://os.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://gr.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jv.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zh.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://mf.szxytkj.cn

Py:   Counter(arr)
来源：http://eg.szsharing.cn

PHP:  array_count_values($arr);
来源：http://qr.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eu.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bw.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qt.colortex.cn

Go:   // 手写 map[T]int
来源：http://pu.hahajie.cn

Ruby: arr.tally
来源：http://dr.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zf.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://kb.huixiangedu.cn

Py:   x in arr
来源：http://we.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://pj.9csxet.cn

JS:   arr.includes(x)
来源：http://bs.shxzskj.cn

TS:   arr.includes(x)
来源：http://ow.521024.cn

Java: list.contains(x)
来源：http://hb.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://ks.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://tz.muxihuayi.cn

C#:   list.Contains(x)
来源：http://zb.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://uj.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fh.shxzukj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bv.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pr.huixiangedu.cn

TS:   [...arr];
来源：http://vd.521024.cn

Java: new ArrayList<>(list);
来源：http://iv.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vp.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://li.huixiangedu.cn

C#:   new List<int>(list);
来源：http://yf.gzmigu.cn

[D23] reduce 累积计算
来源：http://cw.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tp.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nz.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pf.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pd.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pp.521024.cn

Go:   // 手写循环
来源：http://yw.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gf.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tw.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://zz.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rc.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mj.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ra.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rk.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nu.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kb.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bn.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fc.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://el.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nd.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://np.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yz.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wc.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mr.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qf.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://an.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://li.newstarts.cn

[D26] 数组转字符串
来源：http://fo.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://kz.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://wy.muxihuayi.cn

JS:   arr.join(", ")
来源：http://ue.newstarts.cn

TS:   arr.join(", ")
来源：http://fo.nicolike.cn

Java: String.join(", ", list)
来源：http://zs.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://ev.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://xf.521024.cn

C#:   string.Join(", ", list)
来源：http://jr.huixiangedu.cn


<!-- 参考信息 -->