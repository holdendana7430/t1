代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://kd.chemitech.net.cn

TS:   [...a, ...b];
来源：http://he.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fa.lnxyls.cn

Go:   append(a, b...)
来源：http://uk.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://qm.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://rx.bookmarksfly.cn

[D09] 排序（升序）
来源：http://ce.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://so.nicolike.cn

PHP:  sort($arr);
来源：http://lc.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ah.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://an.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://au.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sl.gzmigu.cn

Ruby: arr.sort
来源：http://gc.yuexingan06.cn

C#:   list.Sort();
来源：http://se.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://by.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zb.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lt.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fa.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yz.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oz.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hu.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eq.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jo.nicolike.cn

[D11] 反转数组
来源：http://sq.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yo.hahajie.cn

PHP:  array_reverse($arr);
来源：http://ov.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zi.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://oa.nicolike.cn

Java: Collections.reverse(list);
来源：http://uf.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://wz.hnjuh.cn

Ruby: arr.reverse
来源：http://ge.shxzskj.cn

C#:   list.Reverse();
来源：http://mz.gzmigu.cn

[D12] 查找元素下标
来源：http://cn.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://mn.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pr.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oe.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rj.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mk.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://cs.huixiangedu.cn

Ruby: arr.index(x)
来源：http://kb.szxytkj.cn

C#:   list.IndexOf(x);
来源：http://cb.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://lh.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gb.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pt.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://pg.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://xg.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lf.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jm.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qk.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://np.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://mi.nicolike.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hj.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://es.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://wc.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://er.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yu.huanxung.cn

Go:   // 手写循环
来源：http://pq.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mx.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ts.hnjuh.cn

[D15] 去重
来源：http://gz.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gl.nicolike.cn

PHP:  array_unique($arr);
来源：http://cm.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://ru.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://hb.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hf.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://el.shxzskj.cn

Ruby: arr.uniq
来源：http://we.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://eo.nicolike.cn

[D16] 求和与平均值
来源：http://uy.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ar.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bu.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dp.yuntaijiaju.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xk.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pg.panjiajie.cn

Go:   // 手写循环累加
来源：http://tx.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cx.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://sn.521024.cn

[D17] 最大值与最小值
来源：http://wt.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://kf.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://ib.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zd.szsharing.cn

TS:   Math.max(...arr);
来源：http://um.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pt.521024.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xj.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://dt.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://vj.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://rh.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://df.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://dd.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hh.9csxet.cn

TS:   nested.flat();
来源：http://xw.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nj.wgjwhj.cn

Go:   // 手写双层循环
来源：http://bx.asd995.cn

Ruby: nested.flatten
来源：http://cm.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vg.huixiangedu.cn

[D19] 按字段分组
来源：http://cf.newstarts.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pi.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wy.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qf.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ja.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gz.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://ts.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gy.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vr.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://hu.szxytkj.cn

Py:   Counter(arr)
来源：http://ue.nszjky.cn

PHP:  array_count_values($arr);
来源：http://ik.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bo.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uy.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nw.nicolike.cn

Go:   // 手写 map[T]int
来源：http://lz.colortex.cn

Ruby: arr.tally
来源：http://el.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yh.newstarts.cn

[D21] 判断是否包含某元素
来源：http://no.bookmarksfly.cn

Py:   x in arr
来源：http://ub.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://xh.colortex.cn

JS:   arr.includes(x)
来源：http://jk.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://gl.lnxyls.cn

Java: list.contains(x)
来源：http://gc.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://lh.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://so.chemitech.net.cn

C#:   list.Contains(x)
来源：http://yo.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://at.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qi.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jo.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cs.shtwfgs.cn

TS:   [...arr];
来源：http://as.asd995.cn

Java: new ArrayList<>(list);
来源：http://pe.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rj.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://ja.521024.cn

C#:   new List<int>(list);
来源：http://wa.hahajie.cn

[D23] reduce 累积计算
来源：http://au.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eb.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ow.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eq.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jr.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yu.lnxyls.cn

Go:   // 手写循环
来源：http://nw.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://to.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://us.shxzskj.cn

[D24] 字典 / Map 基本操作
来源：http://ek.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ak.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://es.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nf.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://df.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://te.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bh.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://au.hnjuh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dc.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://rz.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cf.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lf.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wy.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ol.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fp.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ye.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pd.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yj.nszjky.cn

[D26] 数组转字符串
来源：http://ud.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://hx.colortex.cn

PHP:  implode(", ", $arr);
来源：http://hx.huanxung.cn

JS:   arr.join(", ")
来源：http://hf.colortex.cn

TS:   arr.join(", ")
来源：http://mf.bjjhwx.cn

Java: String.join(", ", list)
来源：http://in.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://kt.szxytkj.cn

Ruby: arr.join(", ")
来源：http://xj.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://sa.gzmigu.cn

================================================================================
来源：http://op.haigaiapp.cn

E. 字符串处理
来源：http://nl.shxzskj.cn

================================================================================
来源：http://tx.asd995.cn

[E01] 拼接字符串
来源：http://ef.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ii.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://za.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hp.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zy.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fj.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sp.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pl.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ww.szsharing.cn

[E02] 重复字符串
来源：http://rw.gzmigu.cn

Py:   "ab" * 3
来源：http://fb.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://vv.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://yi.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://ke.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://hd.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://zc.shtwfgs.cn

Ruby: "ab" * 3
来源：http://wl.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vh.panjiajie.cn

[E03] 截取子串
来源：http://gq.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iz.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dj.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qz.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://so.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://jo.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kq.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qi.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://ux.huanxung.cn

[E04] 查找子串位置
来源：http://op.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://qu.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://rw.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ny.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://zw.hnjuh.cn

Java: s.indexOf("x")
来源：http://yk.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://cy.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://rs.521024.cn

C#:   s.IndexOf("x")
来源：http://lf.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tn.wgjwhj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ym.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pg.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ly.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ey.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vx.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tb.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fk.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uu.9csxet.cn

[E06] 替换子串
来源：http://oq.wgjwhj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gx.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://kx.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fz.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://dq.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sy.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ty.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ao.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://dj.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://wc.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wu.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uw.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ui.chemitech.net.cn

TS:   s.split(",")
来源：http://fw.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zi.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jy.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://zj.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uf.szsharing.cn

[E08] 数组按分隔符合并
来源：http://jw.jctech888.com.cn

Py:   ",".join(items)
来源：http://hj.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://ld.huanxung.cn

JS:   items.join(",")
来源：http://nk.szxytkj.cn

TS:   items.join(",")
来源：http://cq.szsharing.cn

Java: String.join(",", items)
来源：http://lh.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://lu.asd995.cn

Ruby: items.join(",")
来源：http://su.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://sx.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://yr.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qq.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nk.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://dx.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://hx.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://kz.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://eh.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jv.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xl.haigaiapp.cn

[E10] 左侧补零 / 定长填充
来源：http://cv.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lu.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qy.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://vt.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://iq.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://wa.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bq.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ja.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ge.huixiangedu.cn

[E11] 反转字符串
来源：http://ar.muxihuayi.cn

Py:   s[::-1]
来源：http://lw.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://pa.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://hq.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://lw.huixiangedu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mg.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://na.shxzukj.cn

Ruby: s.reverse
来源：http://yf.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ey.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://du.szsharing.cn

Py:   s.count("a")
来源：http://nc.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://nc.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://kd.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://jg.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://de.asd995.cn

Go:   strings.Count(s, "a")
来源：http://qn.bjjhwx.cn

Ruby: s.count("a")
来源：http://vv.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://nr.muxihuayi.cn

[E13] 逐字符遍历
来源：http://dt.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://sw.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wy.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qr.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ww.hahajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kj.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://go.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ly.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nr.asd995.cn

[E14] URL 编码与 Base64
来源：http://ef.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ah.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qd.shtwfgs.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://us.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://as.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://po.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tz.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uj.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qa.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://il.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zw.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hx.huanxung.cn


<!-- 参考信息 -->