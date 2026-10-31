代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://pw.9csxet.cn

[D08] 合并两个数组
来源：http://vd.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://bd.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://ro.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ml.chemitech.net.cn

TS:   [...a, ...b];
来源：http://lm.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ru.haigaiapp.cn

Go:   append(a, b...)
来源：http://nf.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://aj.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://ng.chemitech.net.cn

[D09] 排序（升序）
来源：http://zq.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://de.jctech888.com.cn

PHP:  sort($arr);
来源：http://is.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://la.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mf.nicolike.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ex.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gx.nicolike.cn

Ruby: arr.sort
来源：http://gm.shxzukj.cn

C#:   list.Sort();
来源：http://xp.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://il.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ht.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qh.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kj.huixiangedu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bk.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wu.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nc.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://no.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tc.huixiangedu.cn

[D11] 反转数组
来源：http://pc.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hh.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://al.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nu.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://pa.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://yj.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://hd.9csxet.cn

Ruby: arr.reverse
来源：http://fg.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://yg.wgjwhj.cn

[D12] 查找元素下标
来源：http://xp.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://wv.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gi.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vv.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mp.nszjky.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qr.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://ej.bjjhwx.cn

Ruby: arr.index(x)
来源：http://cw.9csxet.cn

C#:   list.IndexOf(x);
来源：http://pr.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://cz.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cy.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gg.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://vu.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://ck.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ru.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iv.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mu.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sz.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://vj.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hr.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yi.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://ia.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://qe.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ac.9csxet.cn

Go:   // 手写循环
来源：http://zh.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uc.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mr.asd995.cn

[D15] 去重
来源：http://pp.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xz.shxzukj.cn

PHP:  array_unique($arr);
来源：http://iw.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://oi.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://jh.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ib.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://el.asd995.cn

Ruby: arr.uniq
来源：http://co.521024.cn

C#:   list.Distinct().ToList()
来源：http://hn.chemitech.net.cn

[D16] 求和与平均值
来源：http://bg.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fo.huixinmuqiang.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gg.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nb.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ou.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://co.muxihuayi.cn

Go:   // 手写循环累加
来源：http://fk.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xc.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://gd.hnjuh.cn

[D17] 最大值与最小值
来源：http://zh.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://wv.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://hw.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vc.panjiajie.cn

TS:   Math.max(...arr);
来源：http://cj.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fs.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nd.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://cl.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://qk.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://au.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://va.asd995.cn

PHP:  array_merge(...$nested);
来源：http://ny.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kl.nicolike.cn

TS:   nested.flat();
来源：http://jm.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qh.shxzskj.cn

Go:   // 手写双层循环
来源：http://bw.bjjhwx.cn

Ruby: nested.flatten
来源：http://on.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kn.nszjky.cn

[D19] 按字段分组
来源：http://ej.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nc.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xj.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zf.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://we.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://un.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://qn.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sj.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yd.521024.cn

[D20] 统计每个元素出现次数
来源：http://nb.shxzukj.cn

Py:   Counter(arr)
来源：http://vt.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://gn.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kc.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wo.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qj.asd995.cn

Go:   // 手写 map[T]int
来源：http://hm.chemitech.net.cn

Ruby: arr.tally
来源：http://cu.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jr.9csxet.cn

[D21] 判断是否包含某元素
来源：http://sm.gzmigu.cn

Py:   x in arr
来源：http://im.shtwfgs.cn

PHP:  in_array($x, $arr, true);
来源：http://ez.colortex.cn

JS:   arr.includes(x)
来源：http://qa.wgjwhj.cn

TS:   arr.includes(x)
来源：http://pq.shxzukj.cn

Java: list.contains(x)
来源：http://df.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://zf.panjiajie.cn

Ruby: arr.include?(x)
来源：http://ps.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://li.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://kr.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dw.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ox.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fu.jianghongdianzi.cn

TS:   [...arr];
来源：http://ig.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://ox.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lp.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://am.haigaiapp.cn

C#:   new List<int>(list);
来源：http://ez.yuexingan06.cn

[D23] reduce 累积计算
来源：http://oe.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qz.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gq.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kd.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://en.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wc.panjiajie.cn

Go:   // 手写循环
来源：http://zg.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pw.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vp.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://nv.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ob.9csxet.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://al.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yk.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sz.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ee.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://or.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tf.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oj.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://ki.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://am.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pp.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dq.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aq.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wm.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qm.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xc.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lt.jianghongdianzi.cn

[D26] 数组转字符串
来源：http://mj.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://od.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://hc.haigaiapp.cn

JS:   arr.join(", ")
来源：http://zf.muxihuayi.cn

TS:   arr.join(", ")
来源：http://pc.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://xc.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://yq.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://zb.nicolike.cn

C#:   string.Join(", ", list)
来源：http://af.gzmigu.cn

================================================================================
来源：http://wd.521024.cn

E. 字符串处理
来源：http://wz.hahajie.cn

================================================================================
来源：http://ao.huanxung.cn

[E01] 拼接字符串
来源：http://ho.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rp.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xd.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eg.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://up.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ts.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vv.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bn.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rm.shxzukj.cn

[E02] 重复字符串
来源：http://za.gzmigu.cn

Py:   "ab" * 3
来源：http://rz.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://hj.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://au.szsharing.cn

TS:   "ab".repeat(3)
来源：http://fp.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://zc.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://ow.shtwfgs.cn

Ruby: "ab" * 3
来源：http://gp.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wg.hahajie.cn

[E03] 截取子串
来源：http://yi.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zr.panjiajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qw.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iu.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://vi.shxzskj.cn

Java: s.substring(1, 4)
来源：http://vl.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kd.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wh.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://bp.colortex.cn

[E04] 查找子串位置
来源：http://jh.szsharing.cn

Py:   s.find("x");  s.index("x")
来源：http://vk.szsharing.cn

PHP:  strpos($s, "x");
来源：http://qi.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dv.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://jt.jctech888.com.cn

Java: s.indexOf("x")
来源：http://fr.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://nm.chemitech.net.cn

Ruby: s.index("x")
来源：http://np.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://mp.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kt.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qe.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vx.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cb.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ul.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ms.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dr.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qk.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ag.bookmarksfly.cn

[E06] 替换子串
来源：http://wb.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://go.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://za.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bi.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://qb.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://as.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dy.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bp.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://at.9csxet.cn

[E07] 按分隔符拆分
来源：http://gy.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mp.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dz.yuexingan06.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ki.muxihuayi.cn

TS:   s.split(",")
来源：http://uo.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xm.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bb.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://aw.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kd.newstarts.cn

[E08] 数组按分隔符合并
来源：http://pe.wgjwhj.cn

Py:   ",".join(items)
来源：http://vf.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://ro.hahajie.cn

JS:   items.join(",")
来源：http://en.wgjwhj.cn

TS:   items.join(",")
来源：http://tv.shtwfgs.cn

Java: String.join(",", items)
来源：http://ul.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://nz.hahajie.cn

Ruby: items.join(",")
来源：http://ln.szxytkj.cn

C#:   string.Join(",", items)
来源：http://qc.szxytkj.cn

[E09] 去除所有空白字符
来源：http://qv.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ry.huixinmuqiang.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vv.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://jk.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://wk.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://ly.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://je.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://im.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ft.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://br.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gd.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dl.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://et.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://qt.nicolike.cn

Java: String.format("%03d", 7)
来源：http://yq.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vu.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dq.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yv.521024.cn

[E11] 反转字符串
来源：http://mo.szsharing.cn

Py:   s[::-1]
来源：http://vo.shxzskj.cn

PHP:  strrev($s);
来源：http://nc.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://zn.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://fr.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yu.huixiangedu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ri.chemitech.net.cn

Ruby: s.reverse
来源：http://yo.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ko.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://xk.newstarts.cn

Py:   s.count("a")
来源：http://pz.yuexingan06.cn

PHP:  substr_count($s, "a");
来源：http://fg.nszjky.cn

JS:   s.split("a").length - 1
来源：http://gi.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://zj.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://au.colortex.cn

Go:   strings.Count(s, "a")
来源：http://io.huixiangedu.cn

Ruby: s.count("a")
来源：http://gm.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://yv.wgjwhj.cn

[E13] 逐字符遍历
来源：http://ts.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://ia.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uf.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jq.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yd.9csxet.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ie.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ln.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vu.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jy.muxihuayi.cn

[E14] URL 编码与 Base64
来源：http://jg.panjiajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gj.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gx.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://og.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eu.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ky.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xp.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iv.nszjky.cn


<!-- 参考信息 -->