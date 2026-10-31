代发 wailian999

[C14] 泛型函数
来源：http://cb.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eb.hnjuh.cn

PHP:  // 无泛型
来源：http://dw.bookmarksfly.cn

JS:   // 无泛型
来源：http://ac.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ra.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ep.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sj.huixiangedu.cn

Ruby: # 无泛型
来源：http://dk.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yl.nicolike.cn

[C15] 解构 / 展开参数
来源：http://tb.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://va.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://kz.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hw.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qw.wgjwhj.cn

Java: // 无解构
来源：http://pr.huixinmuqiang.cn

Go:   // 无解构
来源：http://vt.bjjhwx.cn

Ruby: a, b = pair
来源：http://js.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://ox.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://tb.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sf.yuexingan06.cn

PHP:  // 无重载
来源：http://hb.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rq.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://xq.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pw.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://po.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://ot.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rt.521024.cn

================================================================================
来源：http://jn.colortex.cn

D. 数组 / 列表 / 集合
来源：http://wy.jianghongdianzi.cn

================================================================================
来源：http://yj.szsharing.cn

[D01] 创建数组 / 列表
来源：http://fj.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ut.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cr.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yf.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qo.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bx.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://lk.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://eh.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://et.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://kt.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dk.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ye.shxzskj.cn

JS:   arr.push(4);
来源：http://hx.wgjwhj.cn

TS:   arr.push(4);
来源：http://nr.jctech888.com.cn

Java: list.add(4);
来源：http://ds.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://ol.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://se.9csxet.cn

C#:   list.Add(4);
来源：http://op.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://wx.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://ba.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gh.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ny.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://py.lnxyls.cn

Java: list.add(0, 0);
来源：http://wd.muxihuayi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gc.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vw.colortex.cn

C#:   list.Insert(0, 0);
来源：http://wk.newstarts.cn

[D04] 删除元素
来源：http://ae.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tt.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dt.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ns.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://nn.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vo.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gw.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xk.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wk.chemitech.net.cn

[D05] 访问与修改元素
来源：http://rf.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jx.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hn.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://un.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://ih.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://ee.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://xl.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ro.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sy.521024.cn

[D06] 数组长度
来源：http://qd.jctech888.com.cn

Py:   len(arr)
来源：http://uf.gzmigu.cn

PHP:  count($arr);
来源：http://vd.asd995.cn

JS:   arr.length
来源：http://by.nicolike.cn

TS:   arr.length
来源：http://ph.szsharing.cn

Java: list.size();
来源：http://pd.asd995.cn

Go:   len(arr)
来源：http://sb.huanxung.cn

Ruby: arr.length; arr.size
来源：http://iz.jianghongdianzi.cn

C#:   list.Count;
来源：http://ea.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://jw.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://er.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yg.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://md.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://wu.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://mi.shxzskj.cn

Go:   arr[1:4]
来源：http://pu.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://df.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://pg.yuexingan06.cn

[D08] 合并两个数组
来源：http://bt.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://sl.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://pl.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rk.hahajie.cn

TS:   [...a, ...b];
来源：http://xe.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ee.hahajie.cn

Go:   append(a, b...)
来源：http://bf.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://tu.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://am.nszjky.cn

[D09] 排序（升序）
来源：http://ye.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://tb.szxytkj.cn

PHP:  sort($arr);
来源：http://kt.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kh.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gw.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ix.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yx.chemitech.net.cn

Ruby: arr.sort
来源：http://zq.wgjwhj.cn

C#:   list.Sort();
来源：http://tu.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rl.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xb.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ci.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://im.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ef.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fo.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://db.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://de.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rf.shxzukj.cn

[D11] 反转数组
来源：http://vp.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bp.newstarts.cn

PHP:  array_reverse($arr);
来源：http://tq.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oi.9csxet.cn

TS:   [...arr].reverse();
来源：http://ch.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://rf.colortex.cn

Go:   slices.Reverse(arr)
来源：http://mh.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://rp.521024.cn

C#:   list.Reverse();
来源：http://yp.nicolike.cn

[D12] 查找元素下标
来源：http://ws.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://nj.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fl.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zj.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sv.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hd.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://vp.jctech888.com.cn

Ruby: arr.index(x)
来源：http://rl.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://fz.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://hl.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jm.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oc.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://yt.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://gt.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pk.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ck.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://px.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cx.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://rs.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ln.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fe.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://cn.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://zk.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pu.huixiangedu.cn

Go:   // 手写循环
来源：http://rt.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xy.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://to.shtwfgs.cn

[D15] 去重
来源：http://ie.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ns.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://hx.szsharing.cn

JS:   [...new Set(arr)]
来源：http://rs.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://bf.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nl.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xx.asd995.cn

Ruby: arr.uniq
来源：http://tc.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://yo.bookmarksfly.cn

[D16] 求和与平均值
来源：http://qt.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sh.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zc.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bl.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fp.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://is.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://ux.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ml.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://br.asd995.cn

[D17] 最大值与最小值
来源：http://ca.521024.cn

Py:   max(arr);  min(arr)
来源：http://sj.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://rl.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wf.hahajie.cn

TS:   Math.max(...arr);
来源：http://bk.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gr.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qq.asd995.cn

Ruby: arr.max;  arr.min
来源：http://nv.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://yf.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://wb.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tp.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://gl.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ei.wgjwhj.cn

TS:   nested.flat();
来源：http://lp.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zb.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://yu.hahajie.cn

Ruby: nested.flatten
来源：http://hk.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xk.lnxyls.cn

[D19] 按字段分组
来源：http://xa.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iq.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uq.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pi.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qa.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nh.hahajie.cn

Go:   // 手写 map[string][]T
来源：http://kp.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yw.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jp.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://pm.hahajie.cn

Py:   Counter(arr)
来源：http://xm.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://gn.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nx.huixinmuqiang.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dl.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xv.521024.cn

Go:   // 手写 map[T]int
来源：http://cd.shxzskj.cn

Ruby: arr.tally
来源：http://au.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ko.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://sz.nszjky.cn

Py:   x in arr
来源：http://qa.shtwfgs.cn

PHP:  in_array($x, $arr, true);
来源：http://wl.asd995.cn

JS:   arr.includes(x)
来源：http://hf.shtwfgs.cn

TS:   arr.includes(x)
来源：http://nn.yuexingan06.cn

Java: list.contains(x)
来源：http://dw.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://em.newstarts.cn

Ruby: arr.include?(x)
来源：http://pt.panjiajie.cn

C#:   list.Contains(x)
来源：http://hn.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://xh.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bb.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bp.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hv.szxytkj.cn

TS:   [...arr];
来源：http://ma.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://cn.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xc.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://kx.hahajie.cn

C#:   new List<int>(list);
来源：http://vb.shtwfgs.cn

[D23] reduce 累积计算
来源：http://vu.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xr.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iq.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://se.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ia.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ie.bookmarksfly.cn

Go:   // 手写循环
来源：http://as.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qr.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dy.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://zy.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hc.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pz.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qb.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dv.panjiajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ii.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bl.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bf.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ao.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://gu.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rz.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://md.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ej.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dn.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lo.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mb.shxzukj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hm.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yu.szxytkj.cn

[D26] 数组转字符串
来源：http://nc.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://tv.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://wh.chemitech.net.cn

JS:   arr.join(", ")
来源：http://fu.hnjuh.cn

TS:   arr.join(", ")
来源：http://rr.muxihuayi.cn

Java: String.join(", ", list)
来源：http://je.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://bh.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://zv.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://zq.huixiangedu.cn

================================================================================
来源：http://kq.shxzskj.cn

E. 字符串处理
来源：http://fz.shxzskj.cn

================================================================================
来源：http://aw.9csxet.cn

[E01] 拼接字符串
来源：http://ku.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pl.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zo.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ca.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://km.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ld.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://os.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sl.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vf.gzmigu.cn

[E02] 重复字符串
来源：http://mh.shxzskj.cn

Py:   "ab" * 3
来源：http://ga.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://ab.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://hm.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://tw.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://pk.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://sk.szsharing.cn

Ruby: "ab" * 3
来源：http://ea.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wv.muxihuayi.cn

[E03] 截取子串
来源：http://jv.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zp.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rw.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wy.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://ps.shxzskj.cn

Java: s.substring(1, 4)
来源：http://ab.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jb.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yq.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://gn.gzmigu.cn

[E04] 查找子串位置
来源：http://bm.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://us.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://io.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bm.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://da.shtwfgs.cn

Java: s.indexOf("x")
来源：http://tm.asd995.cn


<!-- 参考信息 -->