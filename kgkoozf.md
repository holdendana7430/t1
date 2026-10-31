代发 wailian999

PHP:  sort($arr);
来源：http://hy.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rz.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cu.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cd.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://af.bookmarksfly.cn

Ruby: arr.sort
来源：http://pc.521024.cn

C#:   list.Sort();
来源：http://cm.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xy.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fr.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aa.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bp.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bb.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ty.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dk.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sd.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lj.shxzskj.cn

[D11] 反转数组
来源：http://gu.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gz.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://tc.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pr.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://zo.colortex.cn

Java: Collections.reverse(list);
来源：http://zu.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://zi.yuexingan06.cn

Ruby: arr.reverse
来源：http://sp.lnxyls.cn

C#:   list.Reverse();
来源：http://ee.huanxung.cn

[D12] 查找元素下标
来源：http://pv.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://ph.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wv.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://up.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tg.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bj.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://rg.lnxyls.cn

Ruby: arr.index(x)
来源：http://vs.521024.cn

C#:   list.IndexOf(x);
来源：http://kj.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://pd.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bf.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ng.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://qo.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://xk.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cl.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sy.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ub.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bj.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://gj.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ut.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cr.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://cp.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://dv.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tg.bookmarksfly.cn

Go:   // 手写循环
来源：http://ds.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sf.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bw.bjjhwx.cn

[D15] 去重
来源：http://ix.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lm.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://ob.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://ib.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://mq.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kl.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qu.521024.cn

Ruby: arr.uniq
来源：http://ky.asd995.cn

C#:   list.Distinct().ToList()
来源：http://dt.hnjuh.cn

[D16] 求和与平均值
来源：http://uq.chemitech.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://to.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ne.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nj.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://he.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://db.nicolike.cn

Go:   // 手写循环累加
来源：http://qd.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qw.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://nf.bjjhwx.cn

[D17] 最大值与最小值
来源：http://wn.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://nk.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://xb.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ro.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://yf.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mg.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pw.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://de.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://ht.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://kl.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bo.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://rp.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nz.lnxyls.cn

TS:   nested.flat();
来源：http://qu.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wp.colortex.cn

Go:   // 手写双层循环
来源：http://mw.nicolike.cn

Ruby: nested.flatten
来源：http://mx.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vo.haigaiapp.cn

[D19] 按字段分组
来源：http://km.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://th.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gl.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uy.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zd.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dr.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://gd.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wp.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xr.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://dm.521024.cn

Py:   Counter(arr)
来源：http://sn.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://ao.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://px.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qw.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aw.szxytkj.cn

Go:   // 手写 map[T]int
来源：http://en.huixiangedu.cn

Ruby: arr.tally
来源：http://mg.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dn.colortex.cn

[D21] 判断是否包含某元素
来源：http://do.panjiajie.cn

Py:   x in arr
来源：http://ol.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://em.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://kv.huixiangedu.cn

TS:   arr.includes(x)
来源：http://od.gzmigu.cn

Java: list.contains(x)
来源：http://sw.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://xs.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://to.gzmigu.cn

C#:   list.Contains(x)
来源：http://zv.shxzskj.cn

[D22] 复制数组（避免共享引用）
来源：http://xk.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kg.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ic.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ec.huanxung.cn

TS:   [...arr];
来源：http://uc.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://de.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ll.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://qr.hahajie.cn

C#:   new List<int>(list);
来源：http://vn.9csxet.cn

[D23] reduce 累积计算
来源：http://zx.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tx.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tp.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sd.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eq.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wg.newstarts.cn

Go:   // 手写循环
来源：http://wi.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jc.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://si.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://ur.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qs.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nd.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pz.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fu.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fl.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fu.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ln.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ff.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://rp.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dg.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pj.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cs.newstarts.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wa.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ub.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://eu.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sr.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pd.newstarts.cn

[D26] 数组转字符串
来源：http://yw.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://ss.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://hy.wgjwhj.cn

JS:   arr.join(", ")
来源：http://dh.newstarts.cn

TS:   arr.join(", ")
来源：http://eo.muxihuayi.cn

Java: String.join(", ", list)
来源：http://vs.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://yj.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://my.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://dp.colortex.cn

================================================================================
来源：http://qy.521024.cn

E. 字符串处理
来源：http://uw.shtwfgs.cn

================================================================================
来源：http://av.yuexingan06.cn

[E01] 拼接字符串
来源：http://lm.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xo.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mc.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ic.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wi.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cs.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fc.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ui.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yd.panjiajie.cn

[E02] 重复字符串
来源：http://jy.jctech888.com.cn

Py:   "ab" * 3
来源：http://rq.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://dt.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://wx.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://tu.gzmigu.cn

Java: "ab".repeat(3)
来源：http://iu.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://jk.hahajie.cn

Ruby: "ab" * 3
来源：http://uk.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hc.bjjhwx.cn

[E03] 截取子串
来源：http://pt.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ih.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ev.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pj.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://wj.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://of.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zd.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://su.colortex.cn

C#:   s.Substring(1, 3)
来源：http://cs.asd995.cn

[E04] 查找子串位置
来源：http://zb.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://ei.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://qv.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sb.lnxyls.cn

TS:   s.indexOf("x")
来源：http://re.chemitech.net.cn

Java: s.indexOf("x")
来源：http://ku.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://ht.asd995.cn

Ruby: s.index("x")
来源：http://le.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://xq.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lm.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qe.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ro.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sp.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gl.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mg.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lt.nicolike.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kz.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jl.panjiajie.cn

[E06] 替换子串
来源：http://mp.wgjwhj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uo.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://ma.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sl.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://uv.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sh.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rb.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ky.521024.cn

C#:   s.Replace("a", "b")
来源：http://ed.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://ks.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ue.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iu.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gd.bookmarksfly.cn

TS:   s.split(",")
来源：http://kx.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hs.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cy.jianghongdianzi.cn

Ruby: s.split(",");  s.split
来源：http://zj.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pc.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://gz.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://tm.asd995.cn

PHP:  implode(",", $items);
来源：http://gd.colortex.cn

JS:   items.join(",")
来源：http://hw.huixiangedu.cn

TS:   items.join(",")
来源：http://tv.szxytkj.cn

Java: String.join(",", items)
来源：http://us.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://dh.panjiajie.cn

Ruby: items.join(",")
来源：http://os.huanxung.cn

C#:   string.Join(",", items)
来源：http://pp.szxytkj.cn

[E09] 去除所有空白字符
来源：http://ex.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://aa.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pd.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://yj.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://tp.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://sd.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yj.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mn.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tv.yuntaijiaju.cn

[E10] 左侧补零 / 定长填充
来源：http://cv.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jg.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cu.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://tl.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://zm.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://vv.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jj.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yy.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ge.haigaiapp.cn

[E11] 反转字符串
来源：http://pa.wgjwhj.cn

Py:   s[::-1]
来源：http://hl.521024.cn

PHP:  strrev($s);
来源：http://nx.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://ej.panjiajie.cn

TS:   [...s].reverse().join("")
来源：http://gg.asd995.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zi.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cs.hnjuh.cn

Ruby: s.reverse
来源：http://nq.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xc.huanxung.cn

[E12] 统计某字符出现次数
来源：http://lo.huixiangedu.cn

Py:   s.count("a")
来源：http://ap.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://ng.9csxet.cn

JS:   s.split("a").length - 1
来源：http://ea.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://sd.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pl.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://dp.panjiajie.cn

Ruby: s.count("a")
来源：http://qx.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://zc.panjiajie.cn

[E13] 逐字符遍历
来源：http://uw.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://zm.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zu.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yh.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qi.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rh.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uu.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fy.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kj.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://nh.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ub.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rr.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kb.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://at.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kh.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cw.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ik.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fa.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://lf.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lm.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vo.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vi.hnjuh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fy.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gp.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wl.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kc.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bj.nszjky.cn

[E16] 数字千分位
来源：http://ul.szsharing.cn

Py:   f"{1234567:,}"
来源：http://lj.shtwfgs.cn


<!-- 参考信息 -->