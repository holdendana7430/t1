代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://cb.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://kg.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://ph.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://ee.shxzskj.cn

PHP:  sort($arr);
来源：http://fq.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://by.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tk.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ui.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lg.panjiajie.cn

Ruby: arr.sort
来源：http://jd.9csxet.cn

C#:   list.Sort();
来源：http://sd.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wy.colortex.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bh.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kn.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pz.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bk.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mz.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qy.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nj.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yx.szxytkj.cn

[D11] 反转数组
来源：http://ky.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wu.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://yp.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qy.colortex.cn

TS:   [...arr].reverse();
来源：http://ok.hahajie.cn

Java: Collections.reverse(list);
来源：http://wk.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://st.bookmarksfly.cn

Ruby: arr.reverse
来源：http://io.hahajie.cn

C#:   list.Reverse();
来源：http://fo.gzmigu.cn

[D12] 查找元素下标
来源：http://vw.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://eq.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://aj.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://go.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iq.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gk.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://zy.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://xu.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://ip.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://sg.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://em.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qi.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://yl.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://he.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qs.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://up.nicolike.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uk.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bq.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://ho.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nb.yuntaijiaju.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sx.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://ad.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://jz.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bk.bookmarksfly.cn

Go:   // 手写循环
来源：http://hd.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pf.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nk.521024.cn

[D15] 去重
来源：http://hs.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ic.nicolike.cn

PHP:  array_unique($arr);
来源：http://tc.colortex.cn

JS:   [...new Set(arr)]
来源：http://co.gzmigu.cn

TS:   [...new Set(arr)]
来源：http://bn.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jm.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rx.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://vv.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://dv.bjjhwx.cn

[D16] 求和与平均值
来源：http://fh.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wh.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tr.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ia.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://no.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hs.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://or.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://di.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://pz.muxihuayi.cn

[D17] 最大值与最小值
来源：http://vx.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://cl.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://ob.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tc.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://bl.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wv.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fr.521024.cn

Ruby: arr.max;  arr.min
来源：http://qb.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://tw.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://mm.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zg.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://ba.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jd.hnjuh.cn

TS:   nested.flat();
来源：http://gv.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vd.shxzukj.cn

Go:   // 手写双层循环
来源：http://wf.shxzskj.cn

Ruby: nested.flatten
来源：http://ip.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wq.yuexingan06.cn

[D19] 按字段分组
来源：http://ux.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://df.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ku.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xb.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ha.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lr.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://fo.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vy.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cc.colortex.cn

[D20] 统计每个元素出现次数
来源：http://co.shtwfgs.cn

Py:   Counter(arr)
来源：http://ih.hahajie.cn

PHP:  array_count_values($arr);
来源：http://hp.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ky.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rp.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kg.colortex.cn

Go:   // 手写 map[T]int
来源：http://ao.newstarts.cn

Ruby: arr.tally
来源：http://dw.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kw.muxihuayi.cn

[D21] 判断是否包含某元素
来源：http://pr.jctech888.com.cn

Py:   x in arr
来源：http://ai.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://ob.haigaiapp.cn

JS:   arr.includes(x)
来源：http://lw.bookmarksfly.cn

TS:   arr.includes(x)
来源：http://as.huixinmuqiang.cn

Java: list.contains(x)
来源：http://ji.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://yk.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://pi.newstarts.cn

C#:   list.Contains(x)
来源：http://ae.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://kf.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nh.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cr.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xb.shxzukj.cn

TS:   [...arr];
来源：http://kl.szsharing.cn

Java: new ArrayList<>(list);
来源：http://zb.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://iu.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://go.newstarts.cn

C#:   new List<int>(list);
来源：http://pq.hnjuh.cn

[D23] reduce 累积计算
来源：http://io.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zu.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bn.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ht.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kb.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pw.asd995.cn

Go:   // 手写循环
来源：http://vj.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bk.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hf.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://jw.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fc.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wu.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hn.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gh.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mi.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bl.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nz.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fw.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://df.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xk.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dj.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ct.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ar.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sb.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oc.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zl.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://so.bjjhwx.cn

[D26] 数组转字符串
来源：http://em.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://hv.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://sj.huanxung.cn

JS:   arr.join(", ")
来源：http://yd.9csxet.cn

TS:   arr.join(", ")
来源：http://xu.huanxung.cn

Java: String.join(", ", list)
来源：http://ye.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://jk.colortex.cn

Ruby: arr.join(", ")
来源：http://nk.szsharing.cn

C#:   string.Join(", ", list)
来源：http://qo.wgjwhj.cn

================================================================================
来源：http://iw.asd995.cn

E. 字符串处理
来源：http://dx.huixinmuqiang.cn

================================================================================
来源：http://xl.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://dn.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ki.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xq.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mt.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cu.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dj.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sa.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://th.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ur.bjjhwx.cn

[E02] 重复字符串
来源：http://na.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://hb.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://am.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://qj.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://om.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://yn.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://hx.nicolike.cn

Ruby: "ab" * 3
来源：http://yd.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xt.nszjky.cn

[E03] 截取子串
来源：http://to.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cx.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nj.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rb.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://yi.szxytkj.cn

Java: s.substring(1, 4)
来源：http://pk.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xn.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zx.panjiajie.cn

C#:   s.Substring(1, 3)
来源：http://iu.hnjuh.cn

[E04] 查找子串位置
来源：http://pd.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://vz.hahajie.cn

PHP:  strpos($s, "x");
来源：http://vt.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zy.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://hv.wgjwhj.cn

Java: s.indexOf("x")
来源：http://uf.asd995.cn

Go:   strings.Index(s, "x")
来源：http://mq.lnxyls.cn

Ruby: s.index("x")
来源：http://kg.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://qo.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ol.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tg.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ui.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oo.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ow.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gy.nicolike.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lr.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vb.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fk.jctech888.com.cn

[E06] 替换子串
来源：http://fn.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://we.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://at.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qf.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://ej.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ye.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pa.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pp.colortex.cn

C#:   s.Replace("a", "b")
来源：http://ww.panjiajie.cn

[E07] 按分隔符拆分
来源：http://eh.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ns.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hh.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://aw.9csxet.cn

TS:   s.split(",")
来源：http://rs.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xq.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fs.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://nt.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cf.huanxung.cn

[E08] 数组按分隔符合并
来源：http://ui.nszjky.cn

Py:   ",".join(items)
来源：http://ov.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://wq.yuntaijiaju.cn

JS:   items.join(",")
来源：http://hg.szsharing.cn

TS:   items.join(",")
来源：http://wt.szxytkj.cn

Java: String.join(",", items)
来源：http://mn.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://la.huanxung.cn

Ruby: items.join(",")
来源：http://mq.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://sp.hahajie.cn

[E09] 去除所有空白字符
来源：http://gg.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pg.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yy.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://jv.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://wp.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://zz.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jm.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tm.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://io.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://fc.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ku.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nf.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://qq.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://pb.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://rv.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://aq.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qo.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yf.huanxung.cn

[E11] 反转字符串
来源：http://dx.huanxung.cn

Py:   s[::-1]
来源：http://bc.hahajie.cn

PHP:  strrev($s);
来源：http://ic.colortex.cn

JS:   [...s].reverse().join("")
来源：http://ab.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://xz.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nw.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://va.wgjwhj.cn

Ruby: s.reverse
来源：http://vb.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gn.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://lq.lnxyls.cn

Py:   s.count("a")
来源：http://qf.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://et.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://sj.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://ug.colortex.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fw.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://vq.huixiangedu.cn

Ruby: s.count("a")
来源：http://at.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://vd.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://xt.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://au.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zh.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ms.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pm.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lr.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pb.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jn.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cu.newstarts.cn

[E14] URL 编码与 Base64
来源：http://tk.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ja.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qn.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vk.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ip.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cm.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uh.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uj.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ag.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://ti.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://au.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gn.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ew.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yg.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tn.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zw.haigaiapp.cn


<!-- 参考信息 -->