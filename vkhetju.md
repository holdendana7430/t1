代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://ji.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://hz.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ei.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://ai.yuntaijiaju.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tz.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jp.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wm.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lv.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://df.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://vr.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ym.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://je.huanxung.cn

[C14] 泛型函数
来源：http://du.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://px.szxytkj.cn

PHP:  // 无泛型
来源：http://cr.9csxet.cn

JS:   // 无泛型
来源：http://tc.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ro.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://go.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ib.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://cj.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ag.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://fr.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ur.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://hl.asd995.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zi.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ur.jianghongdianzi.cn

Java: // 无解构
来源：http://ih.shxzukj.cn

Go:   // 无解构
来源：http://ux.chemitech.net.cn

Ruby: a, b = pair
来源：http://uw.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://vw.nszjky.cn

[C16] 函数 / 方法重载
来源：http://rc.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pd.bookmarksfly.cn

PHP:  // 无重载
来源：http://cg.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pf.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://xa.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wq.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://wy.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://bp.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://go.wgjwhj.cn

================================================================================
来源：http://cd.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://hv.9csxet.cn

================================================================================
来源：http://yc.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://ez.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://py.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qn.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yc.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lx.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wd.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://tr.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://ze.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cw.9csxet.cn

[D02] 追加元素到末尾
来源：http://cr.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ux.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://na.newstarts.cn

JS:   arr.push(4);
来源：http://fl.jctech888.com.cn

TS:   arr.push(4);
来源：http://oz.chemitech.net.cn

Java: list.add(4);
来源：http://ff.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://zf.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://lx.gzmigu.cn

C#:   list.Add(4);
来源：http://xs.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://kn.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://yo.lnxyls.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lh.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://je.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://ts.yuexingan06.cn

Java: list.add(0, 0);
来源：http://rt.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jg.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://la.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://hl.bookmarksfly.cn

[D04] 删除元素
来源：http://zt.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xa.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ys.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gm.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://fa.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ce.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://go.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ug.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pk.521024.cn

[D05] 访问与修改元素
来源：http://dt.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rp.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://se.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xg.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://rd.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://zw.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://vh.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oj.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sl.hnjuh.cn

[D06] 数组长度
来源：http://wb.shxzskj.cn

Py:   len(arr)
来源：http://fg.newstarts.cn

PHP:  count($arr);
来源：http://mn.shxzskj.cn

JS:   arr.length
来源：http://oe.haigaiapp.cn

TS:   arr.length
来源：http://ol.huanxung.cn

Java: list.size();
来源：http://mo.muxihuayi.cn

Go:   len(arr)
来源：http://dp.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://up.szsharing.cn

C#:   list.Count;
来源：http://ww.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://vb.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://od.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ff.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://zz.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://ig.szxytkj.cn

Java: list.subList(1, 4);
来源：http://hj.jctech888.com.cn

Go:   arr[1:4]
来源：http://vx.521024.cn

Ruby: arr[1, 3]
来源：http://ms.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://cx.haigaiapp.cn

[D08] 合并两个数组
来源：http://mw.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://it.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://qe.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vu.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://mf.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bk.nszjky.cn

Go:   append(a, b...)
来源：http://ch.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://ny.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://tq.bjjhwx.cn

[D09] 排序（升序）
来源：http://tw.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://bf.lnxyls.cn

PHP:  sort($arr);
来源：http://wa.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://op.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sl.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fh.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yw.nicolike.cn

Ruby: arr.sort
来源：http://fq.bjjhwx.cn

C#:   list.Sort();
来源：http://xr.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zs.colortex.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oy.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xb.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://td.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fw.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ib.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cr.colortex.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gz.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://td.huixiangedu.cn

[D11] 反转数组
来源：http://sd.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://id.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://yu.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rz.lnxyls.cn

TS:   [...arr].reverse();
来源：http://go.asd995.cn

Java: Collections.reverse(list);
来源：http://kl.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://wr.szsharing.cn

Ruby: arr.reverse
来源：http://bp.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://mn.bookmarksfly.cn

[D12] 查找元素下标
来源：http://ru.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://ox.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mx.nicolike.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zt.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jg.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hg.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://nw.nszjky.cn

Ruby: arr.index(x)
来源：http://mi.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://es.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://zj.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fa.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vc.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://fu.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://lf.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://la.gzmigu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lr.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uk.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nx.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://zd.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ig.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xe.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://uc.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://jv.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://na.521024.cn

Go:   // 手写循环
来源：http://bp.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://su.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cs.huixinmuqiang.cn

[D15] 去重
来源：http://rr.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ov.szxytkj.cn

PHP:  array_unique($arr);
来源：http://ep.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://bf.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://gt.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mk.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://av.bjjhwx.cn

Ruby: arr.uniq
来源：http://pb.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://jw.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://rf.chemitech.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yh.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://md.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vq.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wb.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lc.huanxung.cn

Go:   // 手写循环累加
来源：http://dm.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vp.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://qy.colortex.cn

[D17] 最大值与最小值
来源：http://su.bjjhwx.cn

Py:   max(arr);  min(arr)
来源：http://ee.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://nm.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hj.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://ti.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mf.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ka.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://ci.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://fh.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://lr.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lb.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://pb.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bn.lnxyls.cn

TS:   nested.flat();
来源：http://wn.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zm.jctech888.com.cn

Go:   // 手写双层循环
来源：http://wi.panjiajie.cn

Ruby: nested.flatten
来源：http://pv.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xs.shtwfgs.cn

[D19] 按字段分组
来源：http://ll.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fg.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tr.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iu.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cf.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tt.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://sa.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://au.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uo.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://qe.chemitech.net.cn

Py:   Counter(arr)
来源：http://le.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://wh.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ag.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ax.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://si.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://vl.yuexingan06.cn

Ruby: arr.tally
来源：http://mg.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tu.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://vm.haigaiapp.cn

Py:   x in arr
来源：http://kk.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://cy.jctech888.com.cn

JS:   arr.includes(x)
来源：http://qt.gzmigu.cn

TS:   arr.includes(x)
来源：http://dh.huixinmuqiang.cn

Java: list.contains(x)
来源：http://ns.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://cy.szxytkj.cn

Ruby: arr.include?(x)
来源：http://sr.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://ui.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://ko.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yy.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ak.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://by.yuexingan06.cn

TS:   [...arr];
来源：http://ee.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://kg.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gd.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://yx.jctech888.com.cn

C#:   new List<int>(list);
来源：http://um.szsharing.cn

[D23] reduce 累积计算
来源：http://uu.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ct.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ks.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hp.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qg.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fz.huixiangedu.cn

Go:   // 手写循环
来源：http://gp.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ey.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mv.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://ch.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ua.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://we.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ll.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xw.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ic.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wj.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kb.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tn.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://mq.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kc.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vs.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ru.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jc.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dx.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dh.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://om.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://md.shtwfgs.cn

[D26] 数组转字符串
来源：http://zp.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://gh.jctech888.com.cn

PHP:  implode(", ", $arr);
来源：http://ct.huixiangedu.cn

JS:   arr.join(", ")
来源：http://mp.colortex.cn

TS:   arr.join(", ")
来源：http://kb.haigaiapp.cn

Java: String.join(", ", list)
来源：http://xr.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://ql.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://lc.nszjky.cn

C#:   string.Join(", ", list)
来源：http://ut.wgjwhj.cn

================================================================================
来源：http://pi.bookmarksfly.cn

E. 字符串处理
来源：http://pi.yuexingan06.cn

================================================================================
来源：http://hp.haigaiapp.cn

[E01] 拼接字符串
来源：http://si.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qc.bookmarksfly.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://em.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hh.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ze.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://og.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lf.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ad.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ow.huixinmuqiang.cn

[E02] 重复字符串
来源：http://st.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://vb.jctech888.com.cn

PHP:  str_repeat("ab", 3);
来源：http://nh.hahajie.cn

JS:   "ab".repeat(3)
来源：http://uj.521024.cn

TS:   "ab".repeat(3)
来源：http://cp.9csxet.cn

Java: "ab".repeat(3)
来源：http://zc.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://eo.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://yt.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://un.jctech888.com.cn

[E03] 截取子串
来源：http://az.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wb.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wm.szsharing.cn


<!-- 参考信息 -->