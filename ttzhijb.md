代发 wailian999

PHP:  sort($arr);
来源：http://sk.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rb.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iz.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xo.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zh.hahajie.cn

Ruby: arr.sort
来源：http://rx.newstarts.cn

C#:   list.Sort();
来源：http://tx.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fz.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hh.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fi.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jn.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bc.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dc.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ah.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bj.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nq.muxihuayi.cn

[D11] 反转数组
来源：http://bw.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mt.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://dd.shtwfgs.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vo.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://xa.521024.cn

Java: Collections.reverse(list);
来源：http://gy.asd995.cn

Go:   slices.Reverse(arr)
来源：http://fv.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://zv.muxihuayi.cn

C#:   list.Reverse();
来源：http://hj.shxzskj.cn

[D12] 查找元素下标
来源：http://zt.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://oj.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hm.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vg.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://br.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ct.colortex.cn

Go:   slices.Index(arr, x)
来源：http://zp.gzmigu.cn

Ruby: arr.index(x)
来源：http://lf.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://oj.nszjky.cn

[D13] 过滤（保留满足条件的）
来源：http://hg.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dq.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oa.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://it.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://rd.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tw.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cr.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uk.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xv.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://ka.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nw.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vw.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://mz.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://oo.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pk.hahajie.cn

Go:   // 手写循环
来源：http://eq.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://on.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ly.nszjky.cn

[D15] 去重
来源：http://rv.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ej.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://cr.nicolike.cn

JS:   [...new Set(arr)]
来源：http://zj.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://ji.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yv.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ut.szsharing.cn

Ruby: arr.uniq
来源：http://kg.bookmarksfly.cn

C#:   list.Distinct().ToList()
来源：http://nz.bjjhwx.cn

[D16] 求和与平均值
来源：http://sc.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xc.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://su.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sv.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zp.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wi.haigaiapp.cn

Go:   // 手写循环累加
来源：http://xq.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vv.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://jd.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://fp.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://eo.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://fg.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jz.9csxet.cn

TS:   Math.max(...arr);
来源：http://zv.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lt.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ad.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://pc.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://nu.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://ug.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yc.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://ul.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qs.nszjky.cn

TS:   nested.flat();
来源：http://rk.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hn.hnjuh.cn

Go:   // 手写双层循环
来源：http://iy.nszjky.cn

Ruby: nested.flatten
来源：http://zt.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://df.nszjky.cn

[D19] 按字段分组
来源：http://um.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jx.bookmarksfly.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pz.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ld.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cw.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hb.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://kd.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mz.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eb.colortex.cn

[D20] 统计每个元素出现次数
来源：http://ni.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://lb.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://zj.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ia.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ff.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fc.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://gk.wgjwhj.cn

Ruby: arr.tally
来源：http://gt.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jn.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://xj.bjjhwx.cn

Py:   x in arr
来源：http://ol.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://mr.haigaiapp.cn

JS:   arr.includes(x)
来源：http://kq.colortex.cn

TS:   arr.includes(x)
来源：http://un.yuexingan06.cn

Java: list.contains(x)
来源：http://mc.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://oa.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://zh.yuexingan06.cn

C#:   list.Contains(x)
来源：http://am.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://le.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hv.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vj.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wh.hahajie.cn

TS:   [...arr];
来源：http://yx.newstarts.cn

Java: new ArrayList<>(list);
来源：http://wt.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pr.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://mz.lnxyls.cn

C#:   new List<int>(list);
来源：http://kk.huanxung.cn

[D23] reduce 累积计算
来源：http://ut.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jj.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mr.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://di.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qj.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ve.huixinmuqiang.cn

Go:   // 手写循环
来源：http://ub.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qp.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jz.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://id.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ej.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rw.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ds.colortex.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yb.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wk.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bv.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ck.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nv.521024.cn

[D25] Set 集合去重与交并差
来源：http://cl.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pq.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mm.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lk.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qg.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lu.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vi.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xd.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ey.jctech888.com.cn

[D26] 数组转字符串
来源：http://rw.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://oa.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://hm.huixiangedu.cn

JS:   arr.join(", ")
来源：http://nv.shxzskj.cn

TS:   arr.join(", ")
来源：http://pn.521024.cn

Java: String.join(", ", list)
来源：http://oo.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://co.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://js.521024.cn

C#:   string.Join(", ", list)
来源：http://ho.gzmigu.cn

================================================================================
来源：http://ic.jianghongdianzi.cn

E. 字符串处理
来源：http://on.wgjwhj.cn

================================================================================
来源：http://xz.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://px.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://co.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ix.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tw.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xc.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ih.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aw.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pb.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zl.9csxet.cn

[E02] 重复字符串
来源：http://xd.bookmarksfly.cn

Py:   "ab" * 3
来源：http://qi.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://fn.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://le.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://cm.9csxet.cn

Java: "ab".repeat(3)
来源：http://qf.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://mo.asd995.cn

Ruby: "ab" * 3
来源：http://vh.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fn.521024.cn

[E03] 截取子串
来源：http://nb.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dy.jianghongdianzi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xx.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gn.nicolike.cn

TS:   s.slice(1, 4)
来源：http://hz.szxytkj.cn

Java: s.substring(1, 4)
来源：http://xh.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ml.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tv.panjiajie.cn

C#:   s.Substring(1, 3)
来源：http://nu.hahajie.cn

[E04] 查找子串位置
来源：http://so.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://ru.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://kv.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jf.szsharing.cn

TS:   s.indexOf("x")
来源：http://jy.haigaiapp.cn

Java: s.indexOf("x")
来源：http://wv.asd995.cn

Go:   strings.Index(s, "x")
来源：http://ji.huanxung.cn

Ruby: s.index("x")
来源：http://gb.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://cm.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xu.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cz.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zr.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oj.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nd.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ht.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zr.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eo.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dy.muxihuayi.cn

[E06] 替换子串
来源：http://yz.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ff.colortex.cn

PHP:  str_replace("a", "b", $s);
来源：http://st.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fn.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://nm.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lm.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ci.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nm.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://xo.huanxung.cn

[E07] 按分隔符拆分
来源：http://ly.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xq.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ay.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rf.yuntaijiaju.cn

TS:   s.split(",")
来源：http://zt.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ui.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rg.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://zb.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jv.nicolike.cn

[E08] 数组按分隔符合并
来源：http://ao.wgjwhj.cn

Py:   ",".join(items)
来源：http://if.panjiajie.cn

PHP:  implode(",", $items);
来源：http://sf.521024.cn

JS:   items.join(",")
来源：http://hh.lnxyls.cn

TS:   items.join(",")
来源：http://xl.9csxet.cn

Java: String.join(",", items)
来源：http://bo.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://zq.huixiangedu.cn

Ruby: items.join(",")
来源：http://mb.gzmigu.cn

C#:   string.Join(",", items)
来源：http://qp.szxytkj.cn

[E09] 去除所有空白字符
来源：http://ly.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fp.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tz.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://gl.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://ma.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://rn.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dr.nicolike.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fv.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ps.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://az.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ps.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gu.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://db.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://le.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://hp.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://li.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ga.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hh.jctech888.com.cn

[E11] 反转字符串
来源：http://rq.lnxyls.cn

Py:   s[::-1]
来源：http://au.colortex.cn

PHP:  strrev($s);
来源：http://we.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://ab.panjiajie.cn

TS:   [...s].reverse().join("")
来源：http://hq.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hs.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://if.huixiangedu.cn

Ruby: s.reverse
来源：http://hw.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://is.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://yx.hahajie.cn

Py:   s.count("a")
来源：http://ee.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://uc.huanxung.cn

JS:   s.split("a").length - 1
来源：http://ds.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://gs.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xh.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://eo.haigaiapp.cn

Ruby: s.count("a")
来源：http://ud.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://dr.shtwfgs.cn

[E13] 逐字符遍历
来源：http://ds.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://ks.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xd.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dn.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mp.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nr.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nq.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tl.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yb.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://wf.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://st.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tm.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://es.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wt.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dd.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ic.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sg.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pe.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://cv.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dg.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ni.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ue.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tg.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pf.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bw.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ae.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qf.szxytkj.cn

[E16] 数字千分位
来源：http://rf.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://do.jianghongdianzi.cn


<!-- 参考信息 -->