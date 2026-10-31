代发 wailian999

D. 数组 / 列表 / 集合
来源：http://ie.panjiajie.cn

================================================================================
来源：http://ok.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://ln.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jm.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ez.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yd.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bu.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kj.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://nr.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://qt.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jo.szsharing.cn

[D02] 追加元素到末尾
来源：http://ez.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qn.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zz.gzmigu.cn

JS:   arr.push(4);
来源：http://gz.wgjwhj.cn

TS:   arr.push(4);
来源：http://sj.9csxet.cn

Java: list.add(4);
来源：http://do.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://of.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://im.newstarts.cn

C#:   list.Add(4);
来源：http://ri.nicolike.cn

[D03] 在指定位置插入元素
来源：http://mz.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://ys.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uo.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://em.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://uk.newstarts.cn

Java: list.add(0, 0);
来源：http://ph.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uo.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gv.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://xj.yuexingan06.cn

[D04] 删除元素
来源：http://qr.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://di.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ao.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hh.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://ag.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mi.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ww.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fa.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://at.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://yv.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gc.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ur.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ni.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://cz.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://sj.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://od.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gk.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rq.shxzskj.cn

[D06] 数组长度
来源：http://fl.chemitech.net.cn

Py:   len(arr)
来源：http://gn.lnxyls.cn

PHP:  count($arr);
来源：http://wx.bookmarksfly.cn

JS:   arr.length
来源：http://wr.lnxyls.cn

TS:   arr.length
来源：http://qs.gzmigu.cn

Java: list.size();
来源：http://ss.chemitech.net.cn

Go:   len(arr)
来源：http://fc.huanxung.cn

Ruby: arr.length; arr.size
来源：http://bu.szsharing.cn

C#:   list.Count;
来源：http://nw.szsharing.cn

[D07] 切片 / 取子数组
来源：http://qr.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bc.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://je.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://il.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://et.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://fu.asd995.cn

Go:   arr[1:4]
来源：http://mb.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://ct.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://bu.hahajie.cn

[D08] 合并两个数组
来源：http://og.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://mf.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://bq.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://of.muxihuayi.cn

TS:   [...a, ...b];
来源：http://gw.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bm.shtwfgs.cn

Go:   append(a, b...)
来源：http://lv.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://vx.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://fd.panjiajie.cn

[D09] 排序（升序）
来源：http://dy.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://ir.lnxyls.cn

PHP:  sort($arr);
来源：http://kj.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ve.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://on.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jd.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xg.yuntaijiaju.cn

Ruby: arr.sort
来源：http://kr.bjjhwx.cn

C#:   list.Sort();
来源：http://vm.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oz.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://in.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tn.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qj.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uo.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xm.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xc.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://av.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xa.asd995.cn

[D11] 反转数组
来源：http://bh.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wm.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://ts.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ai.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://gm.hahajie.cn

Java: Collections.reverse(list);
来源：http://xs.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://cm.szsharing.cn

Ruby: arr.reverse
来源：http://wj.9csxet.cn

C#:   list.Reverse();
来源：http://yq.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://ae.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://hq.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fb.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kg.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wf.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ar.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://gb.szxytkj.cn

Ruby: arr.index(x)
来源：http://wn.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://de.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://kd.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ek.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yp.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://ch.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://oo.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ww.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://la.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yc.haigaiapp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hr.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://oz.haigaiapp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dy.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://li.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://hq.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://hw.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rq.panjiajie.cn

Go:   // 手写循环
来源：http://dw.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cb.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://eh.hnjuh.cn

[D15] 去重
来源：http://df.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://in.9csxet.cn

PHP:  array_unique($arr);
来源：http://rs.nicolike.cn

JS:   [...new Set(arr)]
来源：http://yq.gzmigu.cn

TS:   [...new Set(arr)]
来源：http://cz.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wr.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uj.521024.cn

Ruby: arr.uniq
来源：http://bf.bookmarksfly.cn

C#:   list.Distinct().ToList()
来源：http://hx.lnxyls.cn

[D16] 求和与平均值
来源：http://pg.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nh.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hj.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nw.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xk.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ti.lnxyls.cn

Go:   // 手写循环累加
来源：http://lq.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nd.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://pd.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://ji.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://hq.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://ps.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://if.huanxung.cn

TS:   Math.max(...arr);
来源：http://ri.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fe.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yt.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://lw.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://tt.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://nw.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dj.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://np.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rk.huixinmuqiang.cn

TS:   nested.flat();
来源：http://nq.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ds.asd995.cn

Go:   // 手写双层循环
来源：http://bh.panjiajie.cn

Ruby: nested.flatten
来源：http://rm.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fg.wgjwhj.cn

[D19] 按字段分组
来源：http://rm.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tn.lnxyls.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://la.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gk.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qf.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xd.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://sj.hnjuh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jz.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jt.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://uu.chemitech.net.cn

Py:   Counter(arr)
来源：http://co.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://yw.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ed.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://de.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xz.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://kz.bookmarksfly.cn

Ruby: arr.tally
来源：http://py.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nz.hahajie.cn

[D21] 判断是否包含某元素
来源：http://gz.nicolike.cn

Py:   x in arr
来源：http://nt.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://jy.huanxung.cn

JS:   arr.includes(x)
来源：http://av.9csxet.cn

TS:   arr.includes(x)
来源：http://rr.nicolike.cn

Java: list.contains(x)
来源：http://dt.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://rs.newstarts.cn

Ruby: arr.include?(x)
来源：http://gk.haigaiapp.cn

C#:   list.Contains(x)
来源：http://io.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://kz.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ng.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bt.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qo.asd995.cn

TS:   [...arr];
来源：http://nq.521024.cn

Java: new ArrayList<>(list);
来源：http://ji.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kn.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://sh.haigaiapp.cn

C#:   new List<int>(list);
来源：http://ss.muxihuayi.cn

[D23] reduce 累积计算
来源：http://rs.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://up.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tb.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sq.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bs.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dz.muxihuayi.cn

Go:   // 手写循环
来源：http://pz.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kn.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qm.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://aa.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lt.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ag.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cv.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zw.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mi.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jp.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ut.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hj.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://te.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://of.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tw.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://db.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ic.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tf.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xb.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bn.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pv.521024.cn

[D26] 数组转字符串
来源：http://nc.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://kn.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://ie.colortex.cn

JS:   arr.join(", ")
来源：http://li.panjiajie.cn

TS:   arr.join(", ")
来源：http://hc.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://ks.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://sh.hnjuh.cn

Ruby: arr.join(", ")
来源：http://mp.hahajie.cn

C#:   string.Join(", ", list)
来源：http://cg.521024.cn

================================================================================
来源：http://kz.huixiangedu.cn

E. 字符串处理
来源：http://wj.colortex.cn

================================================================================
来源：http://me.wgjwhj.cn

[E01] 拼接字符串
来源：http://ha.521024.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ae.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cs.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ka.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://un.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://np.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xw.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rd.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gw.shxzukj.cn

[E02] 重复字符串
来源：http://at.nicolike.cn

Py:   "ab" * 3
来源：http://xo.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://zp.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://po.hnjuh.cn

TS:   "ab".repeat(3)
来源：http://tf.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://ip.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://qb.gzmigu.cn

Ruby: "ab" * 3
来源：http://ml.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mj.jianghongdianzi.cn

[E03] 截取子串
来源：http://ks.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://as.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oy.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pl.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://eb.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://nt.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sg.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zd.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://os.panjiajie.cn

[E04] 查找子串位置
来源：http://gs.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://qr.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://ch.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://de.nszjky.cn

TS:   s.indexOf("x")
来源：http://wo.hahajie.cn

Java: s.indexOf("x")
来源：http://ac.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://yw.hahajie.cn

Ruby: s.index("x")
来源：http://jb.colortex.cn

C#:   s.IndexOf("x")
来源：http://hn.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://av.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nm.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ix.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yc.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qc.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ww.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dl.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://im.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ao.521024.cn

[E06] 替换子串
来源：http://lr.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vb.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://ec.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fg.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://xj.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zj.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ju.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pu.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://zn.szxytkj.cn

[E07] 按分隔符拆分
来源：http://sx.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jn.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dx.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://aa.yuntaijiaju.cn

TS:   s.split(",")
来源：http://gb.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ak.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ae.hahajie.cn


<!-- 参考信息 -->