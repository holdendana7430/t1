代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://np.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yd.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://rj.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://he.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tl.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ks.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://sx.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://am.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://oa.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qq.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://um.huanxung.cn

[D06] 数组长度
来源：http://sh.gzmigu.cn

Py:   len(arr)
来源：http://py.nszjky.cn

PHP:  count($arr);
来源：http://hn.nicolike.cn

JS:   arr.length
来源：http://fg.szsharing.cn

TS:   arr.length
来源：http://zd.hahajie.cn

Java: list.size();
来源：http://lo.hahajie.cn

Go:   len(arr)
来源：http://rm.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://ep.yuntaijiaju.cn

C#:   list.Count;
来源：http://gb.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://jr.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jt.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vj.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://jr.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://op.szxytkj.cn

Java: list.subList(1, 4);
来源：http://em.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://ip.hnjuh.cn

Ruby: arr[1, 3]
来源：http://xy.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://pd.panjiajie.cn

[D08] 合并两个数组
来源：http://mn.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://iv.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://me.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cy.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://ib.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ug.shxzskj.cn

Go:   append(a, b...)
来源：http://ut.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://zm.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://rj.hnjuh.cn

[D09] 排序（升序）
来源：http://dc.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ex.shxzskj.cn

PHP:  sort($arr);
来源：http://og.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kf.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sg.huanxung.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lp.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qy.colortex.cn

Ruby: arr.sort
来源：http://ni.haigaiapp.cn

C#:   list.Sort();
来源：http://ap.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nx.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://we.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fw.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ob.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bw.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://me.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mb.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://no.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ax.lnxyls.cn

[D11] 反转数组
来源：http://gy.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kh.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://pn.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bl.gzmigu.cn

TS:   [...arr].reverse();
来源：http://bb.szxytkj.cn

Java: Collections.reverse(list);
来源：http://sq.colortex.cn

Go:   slices.Reverse(arr)
来源：http://kd.wgjwhj.cn

Ruby: arr.reverse
来源：http://jt.521024.cn

C#:   list.Reverse();
来源：http://lw.panjiajie.cn

[D12] 查找元素下标
来源：http://pl.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://qn.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://md.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://go.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://an.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zl.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://gi.shxzskj.cn

Ruby: arr.index(x)
来源：http://vv.nicolike.cn

C#:   list.IndexOf(x);
来源：http://ab.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://jt.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ra.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xv.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://ug.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://np.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mo.panjiajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ed.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qv.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uy.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://zb.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wd.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dd.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://sx.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://jm.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gw.lnxyls.cn

Go:   // 手写循环
来源：http://zh.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wr.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ep.wgjwhj.cn

[D15] 去重
来源：http://sk.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bt.panjiajie.cn

PHP:  array_unique($arr);
来源：http://li.nicolike.cn

JS:   [...new Set(arr)]
来源：http://bf.newstarts.cn

TS:   [...new Set(arr)]
来源：http://ts.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ih.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gm.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://cv.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://ph.hahajie.cn

[D16] 求和与平均值
来源：http://ay.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xe.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qg.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rw.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yk.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wh.szxytkj.cn

Go:   // 手写循环累加
来源：http://kf.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jw.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://jn.lnxyls.cn

[D17] 最大值与最小值
来源：http://ll.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://wn.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://hl.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nl.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://vd.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ra.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gs.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://cy.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://wa.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://yi.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://il.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://mx.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xc.muxihuayi.cn

TS:   nested.flat();
来源：http://vv.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zy.newstarts.cn

Go:   // 手写双层循环
来源：http://au.huanxung.cn

Ruby: nested.flatten
来源：http://vh.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hx.haigaiapp.cn

[D19] 按字段分组
来源：http://rx.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://og.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ko.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dx.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ki.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ki.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://eb.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hn.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yd.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://wz.muxihuayi.cn

Py:   Counter(arr)
来源：http://nd.szsharing.cn

PHP:  array_count_values($arr);
来源：http://yx.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aj.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dg.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yl.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://nb.huanxung.cn

Ruby: arr.tally
来源：http://en.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wq.colortex.cn

[D21] 判断是否包含某元素
来源：http://ku.jianghongdianzi.cn

Py:   x in arr
来源：http://kv.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://mj.shtwfgs.cn

JS:   arr.includes(x)
来源：http://yx.panjiajie.cn

TS:   arr.includes(x)
来源：http://bm.hnjuh.cn

Java: list.contains(x)
来源：http://ev.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://jk.asd995.cn

Ruby: arr.include?(x)
来源：http://nx.panjiajie.cn

C#:   list.Contains(x)
来源：http://yj.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://fl.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ei.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wm.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ar.yuntaijiaju.cn

TS:   [...arr];
来源：http://hw.colortex.cn

Java: new ArrayList<>(list);
来源：http://yp.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://iu.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://mm.haigaiapp.cn

C#:   new List<int>(list);
来源：http://ar.bjjhwx.cn

[D23] reduce 累积计算
来源：http://za.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tz.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uv.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bm.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rf.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ie.9csxet.cn

Go:   // 手写循环
来源：http://gc.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qw.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://la.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://dn.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xn.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bv.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ki.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gg.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ye.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oq.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ox.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qz.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://ge.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://na.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xa.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://it.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ki.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wv.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mt.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uy.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cx.shxzskj.cn

[D26] 数组转字符串
来源：http://tq.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://ru.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://sf.shxzukj.cn

JS:   arr.join(", ")
来源：http://ll.szsharing.cn

TS:   arr.join(", ")
来源：http://io.shtwfgs.cn

Java: String.join(", ", list)
来源：http://bq.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://rv.newstarts.cn

Ruby: arr.join(", ")
来源：http://db.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://bt.bookmarksfly.cn

================================================================================
来源：http://gs.hahajie.cn

E. 字符串处理
来源：http://ml.lnxyls.cn

================================================================================
来源：http://ad.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://vb.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xy.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mj.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://er.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eb.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cf.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cm.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kf.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rp.hahajie.cn

[E02] 重复字符串
来源：http://ig.yuexingan06.cn

Py:   "ab" * 3
来源：http://qi.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://wu.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://tz.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://wq.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://fx.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://lz.huixiangedu.cn

Ruby: "ab" * 3
来源：http://mt.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bm.muxihuayi.cn

[E03] 截取子串
来源：http://jx.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oe.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rw.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ws.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://yh.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://ak.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nd.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rm.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://jd.muxihuayi.cn

[E04] 查找子串位置
来源：http://zm.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://pe.szsharing.cn

PHP:  strpos($s, "x");
来源：http://ve.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rg.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://fx.lnxyls.cn

Java: s.indexOf("x")
来源：http://bc.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://uu.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://se.9csxet.cn

C#:   s.IndexOf("x")
来源：http://lq.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cp.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cn.hahajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jd.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bj.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rm.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mf.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hl.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qo.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wz.huixiangedu.cn

[E06] 替换子串
来源：http://ui.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tq.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://gz.nszjky.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://av.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://pj.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ok.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fn.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ve.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://cl.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://lc.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nk.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ks.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dy.yuntaijiaju.cn

TS:   s.split(",")
来源：http://cb.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rp.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zs.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://ax.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vn.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://jp.wgjwhj.cn

Py:   ",".join(items)
来源：http://jr.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://tx.lnxyls.cn

JS:   items.join(",")
来源：http://km.colortex.cn

TS:   items.join(",")
来源：http://lq.nszjky.cn

Java: String.join(",", items)
来源：http://gm.521024.cn

Go:   strings.Join(items, ",")
来源：http://yy.muxihuayi.cn

Ruby: items.join(",")
来源：http://pd.panjiajie.cn

C#:   string.Join(",", items)
来源：http://xv.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://fj.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mz.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://am.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://lw.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://xk.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://qz.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ms.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vz.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nv.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://br.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nc.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hi.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://hc.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://da.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://jy.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pv.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vr.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qk.lnxyls.cn

[E11] 反转字符串
来源：http://ag.chemitech.net.cn

Py:   s[::-1]
来源：http://kq.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://vh.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://hf.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://ya.asd995.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fv.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qj.asd995.cn


<!-- 参考信息 -->