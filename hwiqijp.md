代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://sh.shtwfgs.cn

TS:   [...a, ...b];
来源：http://ka.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ng.bjjhwx.cn

Go:   append(a, b...)
来源：http://tq.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://rc.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://pg.asd995.cn

[D09] 排序（升序）
来源：http://xj.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://hh.asd995.cn

PHP:  sort($arr);
来源：http://se.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dh.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wa.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kh.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lc.gzmigu.cn

Ruby: arr.sort
来源：http://ri.hahajie.cn

C#:   list.Sort();
来源：http://cv.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ps.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zs.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://is.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ol.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oy.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://co.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qr.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://li.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wa.szsharing.cn

[D11] 反转数组
来源：http://tn.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cz.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://hy.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://br.szxytkj.cn

TS:   [...arr].reverse();
来源：http://yu.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://yr.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://fq.bjjhwx.cn

Ruby: arr.reverse
来源：http://se.shxzukj.cn

C#:   list.Reverse();
来源：http://ms.shxzskj.cn

[D12] 查找元素下标
来源：http://ey.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://ox.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dy.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qw.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ud.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xe.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://dc.nicolike.cn

Ruby: arr.index(x)
来源：http://mu.newstarts.cn

C#:   list.IndexOf(x);
来源：http://dt.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://iy.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tu.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://su.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://er.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://mg.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://em.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oq.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://np.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lz.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://he.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gz.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cs.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://vg.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://tl.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rs.huixinmuqiang.cn

Go:   // 手写循环
来源：http://op.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jk.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jn.bjjhwx.cn

[D15] 去重
来源：http://gv.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://aa.szsharing.cn

PHP:  array_unique($arr);
来源：http://gw.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://qn.521024.cn

TS:   [...new Set(arr)]
来源：http://dh.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cj.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lc.wgjwhj.cn

Ruby: arr.uniq
来源：http://lg.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://pa.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://rj.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zl.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wj.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mt.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ge.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bz.huixiangedu.cn

Go:   // 手写循环累加
来源：http://hs.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pt.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://jd.asd995.cn

[D17] 最大值与最小值
来源：http://rc.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://un.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://wl.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gf.shxzukj.cn

TS:   Math.max(...arr);
来源：http://co.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://od.gzmigu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cs.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://mu.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://hf.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://ky.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bf.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://el.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dd.jctech888.com.cn

TS:   nested.flat();
来源：http://jj.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://id.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://cu.colortex.cn

Ruby: nested.flatten
来源：http://uh.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zr.521024.cn

[D19] 按字段分组
来源：http://vj.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ev.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wb.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://al.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://it.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rp.asd995.cn

Go:   // 手写 map[string][]T
来源：http://mi.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jq.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://he.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://yu.521024.cn

Py:   Counter(arr)
来源：http://xp.hahajie.cn

PHP:  array_count_values($arr);
来源：http://pv.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nb.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://or.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sn.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://qm.bookmarksfly.cn

Ruby: arr.tally
来源：http://qd.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fv.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://yv.jctech888.com.cn

Py:   x in arr
来源：http://tp.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://fg.szsharing.cn

JS:   arr.includes(x)
来源：http://cr.newstarts.cn

TS:   arr.includes(x)
来源：http://bj.huixiangedu.cn

Java: list.contains(x)
来源：http://du.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://fy.lnxyls.cn

Ruby: arr.include?(x)
来源：http://qs.bjjhwx.cn

C#:   list.Contains(x)
来源：http://pe.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://ny.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://de.hnjuh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ez.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://op.nicolike.cn

TS:   [...arr];
来源：http://pa.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://ke.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://be.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://qf.nszjky.cn

C#:   new List<int>(list);
来源：http://np.shtwfgs.cn

[D23] reduce 累积计算
来源：http://lm.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://no.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tg.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wj.jianghongdianzi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zw.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cc.haigaiapp.cn

Go:   // 手写循环
来源：http://fd.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yh.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ki.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://kc.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sf.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yb.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://se.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ec.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pr.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ie.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oy.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hk.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://oh.chemitech.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tt.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xf.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lm.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gl.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://se.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ze.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xg.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ul.wgjwhj.cn

[D26] 数组转字符串
来源：http://wb.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://zo.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://gt.hahajie.cn

JS:   arr.join(", ")
来源：http://ni.bjjhwx.cn

TS:   arr.join(", ")
来源：http://jn.asd995.cn

Java: String.join(", ", list)
来源：http://ce.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://ao.521024.cn

Ruby: arr.join(", ")
来源：http://aw.hahajie.cn

C#:   string.Join(", ", list)
来源：http://jq.bjjhwx.cn

================================================================================
来源：http://ru.muxihuayi.cn

E. 字符串处理
来源：http://qj.bjjhwx.cn

================================================================================
来源：http://bo.yuexingan06.cn

[E01] 拼接字符串
来源：http://wt.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yn.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jv.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zk.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wd.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nq.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://do.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xx.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wn.bjjhwx.cn

[E02] 重复字符串
来源：http://aj.asd995.cn

Py:   "ab" * 3
来源：http://dx.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://zi.9csxet.cn

JS:   "ab".repeat(3)
来源：http://nz.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://bk.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://hm.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://ik.shxzskj.cn

Ruby: "ab" * 3
来源：http://sp.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qs.jianghongdianzi.cn

[E03] 截取子串
来源：http://vn.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ok.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zi.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hi.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://hm.lnxyls.cn

Java: s.substring(1, 4)
来源：http://al.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jg.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xe.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://th.shxzukj.cn

[E04] 查找子串位置
来源：http://ex.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://ux.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://ml.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://de.gzmigu.cn

TS:   s.indexOf("x")
来源：http://qr.szxytkj.cn

Java: s.indexOf("x")
来源：http://oh.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://sy.gzmigu.cn

Ruby: s.index("x")
来源：http://eg.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://oz.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uk.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jn.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ed.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ey.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://va.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sn.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qh.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yx.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nq.panjiajie.cn

[E06] 替换子串
来源：http://wr.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qp.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://ha.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vp.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://jo.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xe.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ih.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ui.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://ry.hahajie.cn

[E07] 按分隔符拆分
来源：http://vr.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nr.szsharing.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://im.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://af.lnxyls.cn

TS:   s.split(",")
来源：http://rl.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xt.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oy.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://ur.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kq.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://tk.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://md.panjiajie.cn

PHP:  implode(",", $items);
来源：http://aq.colortex.cn

JS:   items.join(",")
来源：http://rm.nicolike.cn

TS:   items.join(",")
来源：http://hm.yuexingan06.cn

Java: String.join(",", items)
来源：http://cb.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://vx.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://is.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://os.huanxung.cn

[E09] 去除所有空白字符
来源：http://uu.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hw.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sj.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://fa.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://go.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://be.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ur.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://th.wgjwhj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yv.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://fz.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jn.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://se.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://gn.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://zr.newstarts.cn

Java: String.format("%03d", 7)
来源：http://iu.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gd.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pr.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zm.chemitech.net.cn

[E11] 反转字符串
来源：http://dg.muxihuayi.cn

Py:   s[::-1]
来源：http://ke.newstarts.cn

PHP:  strrev($s);
来源：http://rp.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://xf.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://rd.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sj.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ct.newstarts.cn

Ruby: s.reverse
来源：http://ac.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wh.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://kd.colortex.cn

Py:   s.count("a")
来源：http://fp.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://jd.newstarts.cn

JS:   s.split("a").length - 1
来源：http://rc.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://pq.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sl.colortex.cn

Go:   strings.Count(s, "a")
来源：http://lm.shxzukj.cn

Ruby: s.count("a")
来源：http://ev.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://ln.szsharing.cn

[E13] 逐字符遍历
来源：http://uh.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://cd.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://is.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ik.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ky.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dj.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vd.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jb.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cr.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://bh.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kw.jctech888.com.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uf.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gm.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ep.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cl.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nr.muxihuayi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kw.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gf.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://ke.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bm.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://et.jianghongdianzi.cn


<!-- 参考信息 -->