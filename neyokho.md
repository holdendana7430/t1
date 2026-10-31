代发 wailian999

TS:   arr.slice(1, 4);
来源：http://dz.nszjky.cn

Java: list.subList(1, 4);
来源：http://zp.wgjwhj.cn

Go:   arr[1:4]
来源：http://qt.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://sr.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://pj.wgjwhj.cn

[D08] 合并两个数组
来源：http://qp.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://pi.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://kr.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fx.haigaiapp.cn

TS:   [...a, ...b];
来源：http://zr.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xe.newstarts.cn

Go:   append(a, b...)
来源：http://vg.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://um.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://bz.nszjky.cn

[D09] 排序（升序）
来源：http://rp.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://gf.huixiangedu.cn

PHP:  sort($arr);
来源：http://zy.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zh.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uh.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://la.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tw.haigaiapp.cn

Ruby: arr.sort
来源：http://nb.gzmigu.cn

C#:   list.Sort();
来源：http://xb.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ko.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sv.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yo.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wu.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cv.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yp.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fl.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vk.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ea.nicolike.cn

[D11] 反转数组
来源：http://tv.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://de.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://mi.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ol.shxzskj.cn

TS:   [...arr].reverse();
来源：http://kp.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://jw.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://na.shtwfgs.cn

Ruby: arr.reverse
来源：http://hc.newstarts.cn

C#:   list.Reverse();
来源：http://jg.hahajie.cn

[D12] 查找元素下标
来源：http://ea.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://da.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://df.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xp.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pt.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ii.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://dh.bjjhwx.cn

Ruby: arr.index(x)
来源：http://el.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://mr.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://zw.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xo.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mb.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://ss.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://co.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pf.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ii.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xg.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hr.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://pw.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lq.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ia.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://qr.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://ow.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qg.nicolike.cn

Go:   // 手写循环
来源：http://bz.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kx.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uv.haigaiapp.cn

[D15] 去重
来源：http://mb.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lw.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://sl.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://fz.hahajie.cn

TS:   [...new Set(arr)]
来源：http://yp.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yb.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yn.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://bk.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://sy.bjjhwx.cn

[D16] 求和与平均值
来源：http://vi.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fd.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xd.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ah.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kv.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://us.nszjky.cn

Go:   // 手写循环累加
来源：http://tk.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bq.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://mt.hahajie.cn

[D17] 最大值与最小值
来源：http://ob.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://di.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://of.muxihuayi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ad.panjiajie.cn

TS:   Math.max(...arr);
来源：http://xn.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pv.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yu.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://hm.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://qw.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://ml.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ge.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://ax.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fs.huixiangedu.cn

TS:   nested.flat();
来源：http://lo.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zt.bjjhwx.cn

Go:   // 手写双层循环
来源：http://lm.wgjwhj.cn

Ruby: nested.flatten
来源：http://ho.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fl.bookmarksfly.cn

[D19] 按字段分组
来源：http://hp.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ub.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://he.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hk.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wp.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pv.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://uz.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hp.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ui.521024.cn

[D20] 统计每个元素出现次数
来源：http://xj.9csxet.cn

Py:   Counter(arr)
来源：http://zk.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://us.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mr.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wc.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iq.szxytkj.cn

Go:   // 手写 map[T]int
来源：http://nt.bjjhwx.cn

Ruby: arr.tally
来源：http://vx.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cg.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://ax.asd995.cn

Py:   x in arr
来源：http://da.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://mg.nicolike.cn

JS:   arr.includes(x)
来源：http://tm.lnxyls.cn

TS:   arr.includes(x)
来源：http://wv.bjjhwx.cn

Java: list.contains(x)
来源：http://pl.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://ig.newstarts.cn

Ruby: arr.include?(x)
来源：http://pf.huixiangedu.cn

C#:   list.Contains(x)
来源：http://hm.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://oo.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aa.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vw.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nf.szsharing.cn

TS:   [...arr];
来源：http://lk.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://jb.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fh.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://ma.asd995.cn

C#:   new List<int>(list);
来源：http://pb.shxzukj.cn

[D23] reduce 累积计算
来源：http://zf.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gu.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vh.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eg.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tk.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wv.bjjhwx.cn

Go:   // 手写循环
来源：http://tv.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ry.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ik.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://lh.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tk.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ab.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dg.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://py.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ck.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uj.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ex.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qd.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://gf.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gj.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ox.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ie.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eh.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lc.521024.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kw.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dl.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kf.jctech888.com.cn

[D26] 数组转字符串
来源：http://qh.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://tq.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://dz.huixiangedu.cn

JS:   arr.join(", ")
来源：http://vv.yuexingan06.cn

TS:   arr.join(", ")
来源：http://ko.colortex.cn

Java: String.join(", ", list)
来源：http://th.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://gp.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://kn.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://tl.nicolike.cn

================================================================================
来源：http://iv.jctech888.com.cn

E. 字符串处理
来源：http://ga.yuexingan06.cn

================================================================================
来源：http://oo.colortex.cn

[E01] 拼接字符串
来源：http://tm.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://td.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ri.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ei.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tr.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oo.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://as.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lh.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dj.jctech888.com.cn

[E02] 重复字符串
来源：http://dt.chemitech.net.cn

Py:   "ab" * 3
来源：http://tb.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://gb.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://kr.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://ie.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://mp.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://os.shxzskj.cn

Ruby: "ab" * 3
来源：http://uh.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fd.lnxyls.cn

[E03] 截取子串
来源：http://ge.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aw.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://js.colortex.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yj.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://rd.newstarts.cn

Java: s.substring(1, 4)
来源：http://li.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://le.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mb.huixiangedu.cn

C#:   s.Substring(1, 3)
来源：http://ot.nszjky.cn

[E04] 查找子串位置
来源：http://bo.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://nb.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://de.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bm.szxytkj.cn

TS:   s.indexOf("x")
来源：http://zi.wgjwhj.cn

Java: s.indexOf("x")
来源：http://oh.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://cv.shxzukj.cn

Ruby: s.index("x")
来源：http://qr.521024.cn

C#:   s.IndexOf("x")
来源：http://vb.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xy.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zo.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uc.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lx.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ow.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kp.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bb.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xn.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yj.szsharing.cn

[E06] 替换子串
来源：http://ww.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iq.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://ao.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rs.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://wp.asd995.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rl.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tg.asd995.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://as.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://un.szsharing.cn

[E07] 按分隔符拆分
来源：http://gl.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cy.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kw.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://de.gzmigu.cn

TS:   s.split(",")
来源：http://sc.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zr.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vh.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://pw.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fd.bjjhwx.cn

[E08] 数组按分隔符合并
来源：http://ub.bookmarksfly.cn

Py:   ",".join(items)
来源：http://bo.szsharing.cn

PHP:  implode(",", $items);
来源：http://xj.jianghongdianzi.cn

JS:   items.join(",")
来源：http://ws.jctech888.com.cn

TS:   items.join(",")
来源：http://wb.shxzukj.cn

Java: String.join(",", items)
来源：http://fv.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://nd.521024.cn

Ruby: items.join(",")
来源：http://uh.hahajie.cn

C#:   string.Join(",", items)
来源：http://tz.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://ae.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uz.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ih.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://no.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://bg.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://lw.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ha.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fq.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oj.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://ne.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rf.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ms.521024.cn

JS:   "7".padStart(3, "0")
来源：http://yb.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://vl.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://wz.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ds.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qu.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bi.asd995.cn

[E11] 反转字符串
来源：http://dh.huanxung.cn

Py:   s[::-1]
来源：http://fs.521024.cn

PHP:  strrev($s);
来源：http://tj.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://fy.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://ac.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qz.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://om.gzmigu.cn

Ruby: s.reverse
来源：http://rb.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lg.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://bl.panjiajie.cn

Py:   s.count("a")
来源：http://sw.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://xn.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://ql.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://hk.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cr.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://gu.panjiajie.cn

Ruby: s.count("a")
来源：http://uw.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://vv.colortex.cn

[E13] 逐字符遍历
来源：http://sl.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://li.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eu.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://at.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mm.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uu.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tc.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vk.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lh.colortex.cn

[E14] URL 编码与 Base64
来源：http://do.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ks.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tk.hnjuh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cy.lnxyls.cn


<!-- 参考信息 -->