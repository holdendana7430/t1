代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://lv.wgjwhj.cn

C#:   using System.Text;
来源：http://mp.hahajie.cn

[C12] 立即执行函数 IIFE
来源：http://jn.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://ss.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://qr.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://tz.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://hb.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pk.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://ee.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://kz.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://eq.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://hv.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nx.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gs.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vl.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://px.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ee.newstarts.cn

Go:   func add(a, b int) int
来源：http://wv.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://af.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://iq.muxihuayi.cn

[C14] 泛型函数
来源：http://pp.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jo.gzmigu.cn

PHP:  // 无泛型
来源：http://ur.huixinmuqiang.cn

JS:   // 无泛型
来源：http://qp.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://de.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xe.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tf.jctech888.com.cn

Ruby: # 无泛型
来源：http://df.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sa.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://iy.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://di.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://fv.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pb.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gt.haigaiapp.cn

Java: // 无解构
来源：http://as.shxzskj.cn

Go:   // 无解构
来源：http://wm.gzmigu.cn

Ruby: a, b = pair
来源：http://ad.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://fq.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://fj.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ii.9csxet.cn

PHP:  // 无重载
来源：http://fn.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://my.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://sj.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yd.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://kv.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://ml.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://um.yuexingan06.cn

================================================================================
来源：http://pm.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://xq.shxzukj.cn

================================================================================
来源：http://ln.colortex.cn

[D01] 创建数组 / 列表
来源：http://rn.521024.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://et.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wd.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sh.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dt.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ib.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ld.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://uu.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lc.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://mj.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oe.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yt.jctech888.com.cn

JS:   arr.push(4);
来源：http://oe.chemitech.net.cn

TS:   arr.push(4);
来源：http://sb.hnjuh.cn

Java: list.add(4);
来源：http://rl.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://ky.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://vo.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://fl.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://og.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://xe.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://my.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wi.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://kc.hnjuh.cn

Java: list.add(0, 0);
来源：http://bq.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lh.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://io.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://ps.muxihuayi.cn

[D04] 删除元素
来源：http://uw.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ix.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cv.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mu.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://mj.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ua.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wu.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ay.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fp.chemitech.net.cn

[D05] 访问与修改元素
来源：http://rn.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vl.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xu.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://la.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://pg.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://nl.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://mc.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jy.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kk.chemitech.net.cn

[D06] 数组长度
来源：http://tl.huixinmuqiang.cn

Py:   len(arr)
来源：http://sw.9csxet.cn

PHP:  count($arr);
来源：http://be.yuntaijiaju.cn

JS:   arr.length
来源：http://ss.huixinmuqiang.cn

TS:   arr.length
来源：http://sm.nicolike.cn

Java: list.size();
来源：http://st.lnxyls.cn

Go:   len(arr)
来源：http://rt.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://sq.hahajie.cn

C#:   list.Count;
来源：http://ac.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://yk.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lk.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://au.521024.cn

JS:   arr.slice(1, 4);
来源：http://rc.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://ld.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://bc.wgjwhj.cn

Go:   arr[1:4]
来源：http://ce.lnxyls.cn

Ruby: arr[1, 3]
来源：http://is.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://iu.lnxyls.cn

[D08] 合并两个数组
来源：http://gc.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://jg.521024.cn

PHP:  array_merge($a, $b);
来源：http://ew.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wg.yuexingan06.cn

TS:   [...a, ...b];
来源：http://rx.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sz.asd995.cn

Go:   append(a, b...)
来源：http://jl.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://mr.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://as.huanxung.cn

[D09] 排序（升序）
来源：http://jq.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://cm.jctech888.com.cn

PHP:  sort($arr);
来源：http://wy.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://da.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cr.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cp.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yo.wgjwhj.cn

Ruby: arr.sort
来源：http://yt.nicolike.cn

C#:   list.Sort();
来源：http://rh.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tt.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ng.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://we.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gw.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fq.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lw.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ch.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jy.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://la.bookmarksfly.cn

[D11] 反转数组
来源：http://po.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wh.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://ry.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sc.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://ac.hahajie.cn

Java: Collections.reverse(list);
来源：http://qa.colortex.cn

Go:   slices.Reverse(arr)
来源：http://yt.huixiangedu.cn

Ruby: arr.reverse
来源：http://fv.colortex.cn

C#:   list.Reverse();
来源：http://mj.szsharing.cn

[D12] 查找元素下标
来源：http://vg.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://gk.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://by.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wb.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bg.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://xy.muxihuayi.cn

Ruby: arr.index(x)
来源：http://fx.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://go.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://tt.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aq.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bn.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://ut.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://cn.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bo.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yt.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ow.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ml.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://el.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://am.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gx.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://fz.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://mu.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gf.shxzukj.cn

Go:   // 手写循环
来源：http://er.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ir.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xf.hahajie.cn

[D15] 去重
来源：http://on.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://be.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://rb.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://ft.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://st.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lq.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yn.chemitech.net.cn

Ruby: arr.uniq
来源：http://bg.colortex.cn

C#:   list.Distinct().ToList()
来源：http://ta.shtwfgs.cn

[D16] 求和与平均值
来源：http://jt.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qj.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zg.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cr.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lb.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zd.jctech888.com.cn

Go:   // 手写循环累加
来源：http://je.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cr.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://it.chemitech.net.cn

[D17] 最大值与最小值
来源：http://vm.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://ep.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://bv.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xg.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://ub.muxihuayi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bh.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vt.huixinmuqiang.cn

Ruby: arr.max;  arr.min
来源：http://rn.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://rq.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://pd.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bv.colortex.cn

PHP:  array_merge(...$nested);
来源：http://cs.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rw.jianghongdianzi.cn

TS:   nested.flat();
来源：http://yu.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dg.yuexingan06.cn

Go:   // 手写双层循环
来源：http://hj.muxihuayi.cn

Ruby: nested.flatten
来源：http://kk.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ik.panjiajie.cn

[D19] 按字段分组
来源：http://sx.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ge.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pe.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aq.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pa.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gw.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://ut.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://du.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zc.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://da.jctech888.com.cn

Py:   Counter(arr)
来源：http://ig.colortex.cn

PHP:  array_count_values($arr);
来源：http://nu.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gn.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jl.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://js.nicolike.cn

Go:   // 手写 map[T]int
来源：http://mz.wgjwhj.cn

Ruby: arr.tally
来源：http://ut.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qe.521024.cn

[D21] 判断是否包含某元素
来源：http://iz.hahajie.cn

Py:   x in arr
来源：http://fb.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://mf.panjiajie.cn

JS:   arr.includes(x)
来源：http://hx.szsharing.cn

TS:   arr.includes(x)
来源：http://bx.huanxung.cn

Java: list.contains(x)
来源：http://ab.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://xc.nszjky.cn

Ruby: arr.include?(x)
来源：http://rv.bjjhwx.cn

C#:   list.Contains(x)
来源：http://vr.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://fz.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yr.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yv.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jq.asd995.cn

TS:   [...arr];
来源：http://pl.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://tz.chemitech.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ra.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://zo.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://cj.hnjuh.cn

[D23] reduce 累积计算
来源：http://ra.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cz.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xo.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ez.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uf.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lg.yuntaijiaju.cn

Go:   // 手写循环
来源：http://hz.haigaiapp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zm.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ci.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://jf.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jn.asd995.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yg.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rl.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dm.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zf.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tp.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jx.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rt.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://jf.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ec.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zt.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gd.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tx.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ps.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ss.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xo.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yp.jctech888.com.cn

[D26] 数组转字符串
来源：http://ri.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://sz.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://ty.9csxet.cn

JS:   arr.join(", ")
来源：http://hr.yuexingan06.cn

TS:   arr.join(", ")
来源：http://ap.nszjky.cn

Java: String.join(", ", list)
来源：http://gn.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://st.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://ob.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://sn.yuexingan06.cn

================================================================================
来源：http://aj.colortex.cn

E. 字符串处理
来源：http://wh.nszjky.cn

================================================================================
来源：http://zn.shxzskj.cn

[E01] 拼接字符串
来源：http://ip.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wx.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qa.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nz.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mo.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ln.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://al.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ub.hahajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mi.panjiajie.cn

[E02] 重复字符串
来源：http://ek.bjjhwx.cn

Py:   "ab" * 3
来源：http://tj.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://cx.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://ll.hahajie.cn


<!-- 参考信息 -->