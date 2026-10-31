代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ia.9csxet.cn

Ruby: arr.sort
来源：http://ei.huixiangedu.cn

C#:   list.Sort();
来源：http://xg.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fe.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bj.huixinmuqiang.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bw.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rn.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://og.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zu.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://th.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://or.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ik.szxytkj.cn

[D11] 反转数组
来源：http://lg.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uk.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://fm.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eq.huixinmuqiang.cn

TS:   [...arr].reverse();
来源：http://ln.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://dj.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://af.nszjky.cn

Ruby: arr.reverse
来源：http://ab.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://ls.hnjuh.cn

[D12] 查找元素下标
来源：http://iq.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://eu.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lk.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hk.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://re.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hi.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://qa.gzmigu.cn

Ruby: arr.index(x)
来源：http://hp.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://xr.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://wq.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hi.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ht.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://oo.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://ni.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gj.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nn.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ud.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ed.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://bi.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lm.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fy.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://hq.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://xn.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://za.bjjhwx.cn

Go:   // 手写循环
来源：http://ar.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ai.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pr.yuexingan06.cn

[D15] 去重
来源：http://ky.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jb.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://hh.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://fl.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://hp.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rc.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://te.9csxet.cn

Ruby: arr.uniq
来源：http://rr.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://je.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://jg.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ov.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yr.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xe.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jz.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iy.hnjuh.cn

Go:   // 手写循环累加
来源：http://ij.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qb.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://mr.chemitech.net.cn

[D17] 最大值与最小值
来源：http://rd.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://pc.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://fh.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nr.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://sq.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://py.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mr.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://rz.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://ml.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://he.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hk.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://ue.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wp.jianghongdianzi.cn

TS:   nested.flat();
来源：http://kw.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cr.colortex.cn

Go:   // 手写双层循环
来源：http://hz.bookmarksfly.cn

Ruby: nested.flatten
来源：http://nb.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://po.lnxyls.cn

[D19] 按字段分组
来源：http://pm.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nb.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qr.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://np.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ax.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sl.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://tl.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ir.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oh.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://zh.shtwfgs.cn

Py:   Counter(arr)
来源：http://az.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://ff.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gz.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gh.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hc.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://an.shtwfgs.cn

Ruby: arr.tally
来源：http://od.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yr.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://en.521024.cn

Py:   x in arr
来源：http://rc.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://nx.asd995.cn

JS:   arr.includes(x)
来源：http://me.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://wi.hnjuh.cn

Java: list.contains(x)
来源：http://mf.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://yu.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://wv.chemitech.net.cn

C#:   list.Contains(x)
来源：http://ha.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://br.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uu.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yr.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yw.chemitech.net.cn

TS:   [...arr];
来源：http://bv.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://ao.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bf.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://mg.chemitech.net.cn

C#:   new List<int>(list);
来源：http://op.nszjky.cn

[D23] reduce 累积计算
来源：http://ls.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eo.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qg.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zt.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bc.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://be.colortex.cn

Go:   // 手写循环
来源：http://zv.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ak.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nu.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://fd.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://br.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://da.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://se.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jb.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lv.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gz.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ks.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rs.colortex.cn

[D25] Set 集合去重与交并差
来源：http://vw.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://od.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bz.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wr.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://do.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gp.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://un.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ls.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cu.muxihuayi.cn

[D26] 数组转字符串
来源：http://ni.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://sq.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://sj.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://eb.shxzskj.cn

TS:   arr.join(", ")
来源：http://bl.shxzskj.cn

Java: String.join(", ", list)
来源：http://xb.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://kf.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://le.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://tm.bjjhwx.cn

================================================================================
来源：http://od.jctech888.com.cn

E. 字符串处理
来源：http://uc.9csxet.cn

================================================================================
来源：http://fz.wgjwhj.cn

[E01] 拼接字符串
来源：http://oa.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://we.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jn.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wh.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ek.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fv.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nl.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ib.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lw.szxytkj.cn

[E02] 重复字符串
来源：http://dw.huanxung.cn

Py:   "ab" * 3
来源：http://nv.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://gq.szsharing.cn

JS:   "ab".repeat(3)
来源：http://sk.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://mp.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://if.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://ua.nszjky.cn

Ruby: "ab" * 3
来源：http://zx.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xh.szxytkj.cn

[E03] 截取子串
来源：http://xl.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rb.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zo.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uv.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://fz.jctech888.com.cn

Java: s.substring(1, 4)
来源：http://ey.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jl.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qx.521024.cn

C#:   s.Substring(1, 3)
来源：http://ju.shtwfgs.cn

[E04] 查找子串位置
来源：http://pe.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://hj.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://pk.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fw.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://ro.colortex.cn

Java: s.indexOf("x")
来源：http://su.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://cs.bjjhwx.cn

Ruby: s.index("x")
来源：http://so.szsharing.cn

C#:   s.IndexOf("x")
来源：http://hc.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zr.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fr.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://do.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lx.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dy.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xi.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://po.521024.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nd.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cv.jctech888.com.cn

[E06] 替换子串
来源：http://bw.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ip.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://lr.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tb.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://nx.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cn.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gt.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yp.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://ho.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://zs.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dp.szsharing.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://os.9csxet.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://du.gzmigu.cn

TS:   s.split(",")
来源：http://bg.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qc.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xr.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://ew.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://an.colortex.cn

[E08] 数组按分隔符合并
来源：http://ha.shxzukj.cn

Py:   ",".join(items)
来源：http://pa.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://pv.hnjuh.cn

JS:   items.join(",")
来源：http://lq.panjiajie.cn

TS:   items.join(",")
来源：http://mi.9csxet.cn

Java: String.join(",", items)
来源：http://ne.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://eh.521024.cn

Ruby: items.join(",")
来源：http://co.wgjwhj.cn

C#:   string.Join(",", items)
来源：http://ko.9csxet.cn

[E09] 去除所有空白字符
来源：http://sh.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rh.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://st.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://ae.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://rs.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://iv.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mg.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vc.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://em.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://nq.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bg.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tq.newstarts.cn

JS:   "7".padStart(3, "0")
来源：http://fs.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://ii.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://ny.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xd.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yu.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vn.huanxung.cn

[E11] 反转字符串
来源：http://ab.panjiajie.cn

Py:   s[::-1]
来源：http://zv.wgjwhj.cn

PHP:  strrev($s);
来源：http://ml.521024.cn

JS:   [...s].reverse().join("")
来源：http://ak.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://bu.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mw.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zl.9csxet.cn

Ruby: s.reverse
来源：http://ok.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xe.jianghongdianzi.cn

[E12] 统计某字符出现次数
来源：http://uz.colortex.cn

Py:   s.count("a")
来源：http://ry.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://ix.asd995.cn

JS:   s.split("a").length - 1
来源：http://ao.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://si.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sj.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://dr.lnxyls.cn

Ruby: s.count("a")
来源：http://hg.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://fz.jctech888.com.cn

[E13] 逐字符遍历
来源：http://xu.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://ss.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gw.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yc.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ka.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://df.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mb.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dw.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://at.colortex.cn

[E14] URL 编码与 Base64
来源：http://gd.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bi.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zv.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cu.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ru.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hl.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sr.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rh.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qw.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://ry.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zo.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zd.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://st.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zy.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yj.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nc.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xr.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ei.newstarts.cn

[E16] 数字千分位
来源：http://hq.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://bh.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://yz.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ar.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lw.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jk.wgjwhj.cn


<!-- 参考信息 -->