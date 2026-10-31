代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bu.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wy.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zy.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ua.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ao.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mi.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jb.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qg.panjiajie.cn

[D11] 反转数组
来源：http://gj.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wh.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://km.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sb.colortex.cn

TS:   [...arr].reverse();
来源：http://sq.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://oo.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://qw.9csxet.cn

Ruby: arr.reverse
来源：http://nu.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://ys.nicolike.cn

[D12] 查找元素下标
来源：http://rj.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://lg.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rk.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yl.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vi.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qz.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://iu.wgjwhj.cn

Ruby: arr.index(x)
来源：http://nj.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://ah.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://pk.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sz.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tw.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://yb.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://vh.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xb.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ol.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dg.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rv.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://hb.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tq.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ol.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://ff.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://vb.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dk.szsharing.cn

Go:   // 手写循环
来源：http://sy.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qh.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xm.huixiangedu.cn

[D15] 去重
来源：http://dq.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ae.panjiajie.cn

PHP:  array_unique($arr);
来源：http://dd.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://qq.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://od.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xd.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uj.yuexingan06.cn

Ruby: arr.uniq
来源：http://le.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://gc.asd995.cn

[D16] 求和与平均值
来源：http://hw.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pq.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wp.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pq.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dc.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cr.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://hg.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hy.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://tn.shtwfgs.cn

[D17] 最大值与最小值
来源：http://il.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://xm.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://ws.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ra.shxzukj.cn

TS:   Math.max(...arr);
来源：http://pr.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qt.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://df.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://ct.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://sp.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://wx.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qz.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://ca.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vn.asd995.cn

TS:   nested.flat();
来源：http://vl.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wk.huixiangedu.cn

Go:   // 手写双层循环
来源：http://ol.bjjhwx.cn

Ruby: nested.flatten
来源：http://vn.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://eu.bjjhwx.cn

[D19] 按字段分组
来源：http://ts.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oe.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kn.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gm.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://go.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zu.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://uh.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rn.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://id.asd995.cn

[D20] 统计每个元素出现次数
来源：http://ln.huixiangedu.cn

Py:   Counter(arr)
来源：http://uj.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://su.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xc.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fe.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zn.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://hn.panjiajie.cn

Ruby: arr.tally
来源：http://uf.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dr.9csxet.cn

[D21] 判断是否包含某元素
来源：http://fb.nszjky.cn

Py:   x in arr
来源：http://ai.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://yb.asd995.cn

JS:   arr.includes(x)
来源：http://fm.yuexingan06.cn

TS:   arr.includes(x)
来源：http://dl.bookmarksfly.cn

Java: list.contains(x)
来源：http://iv.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://ge.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://ua.nszjky.cn

C#:   list.Contains(x)
来源：http://wz.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://ku.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wy.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hl.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eq.chemitech.net.cn

TS:   [...arr];
来源：http://ma.colortex.cn

Java: new ArrayList<>(list);
来源：http://zb.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qf.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://xp.szxytkj.cn

C#:   new List<int>(list);
来源：http://ja.haigaiapp.cn

[D23] reduce 累积计算
来源：http://ke.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rf.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lj.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ys.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vg.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xw.wgjwhj.cn

Go:   // 手写循环
来源：http://jo.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://st.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rl.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://pe.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fm.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wr.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wr.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jz.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uk.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jr.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gk.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rt.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://nb.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wy.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bl.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dq.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kp.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jt.huanxung.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vl.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ts.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rt.szsharing.cn

[D26] 数组转字符串
来源：http://vb.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://wm.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://wh.shxzukj.cn

JS:   arr.join(", ")
来源：http://hu.nicolike.cn

TS:   arr.join(", ")
来源：http://uc.chemitech.net.cn

Java: String.join(", ", list)
来源：http://hd.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://ad.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://ko.newstarts.cn

C#:   string.Join(", ", list)
来源：http://fi.chemitech.net.cn

================================================================================
来源：http://om.huanxung.cn

E. 字符串处理
来源：http://uh.wgjwhj.cn

================================================================================
来源：http://ef.lnxyls.cn

[E01] 拼接字符串
来源：http://af.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qb.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dg.shtwfgs.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wq.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gs.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://je.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rq.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://by.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ga.huixiangedu.cn

[E02] 重复字符串
来源：http://sb.szsharing.cn

Py:   "ab" * 3
来源：http://ye.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://hv.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://xb.nicolike.cn

TS:   "ab".repeat(3)
来源：http://to.huanxung.cn

Java: "ab".repeat(3)
来源：http://fn.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://la.521024.cn

Ruby: "ab" * 3
来源：http://ja.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zg.shtwfgs.cn

[E03] 截取子串
来源：http://rr.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nl.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ms.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rv.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://lg.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://va.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://th.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bh.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://mh.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://hd.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://ev.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://pn.yuexingan06.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vf.nicolike.cn

TS:   s.indexOf("x")
来源：http://hd.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://ha.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://ov.9csxet.cn

Ruby: s.index("x")
来源：http://qj.nicolike.cn

C#:   s.IndexOf("x")
来源：http://ti.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://eb.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mc.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tb.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ig.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ha.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yh.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://it.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qw.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fb.lnxyls.cn

[E06] 替换子串
来源：http://he.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://re.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://jq.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xg.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://tu.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mq.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uv.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gf.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://xm.gzmigu.cn

[E07] 按分隔符拆分
来源：http://ro.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ap.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jx.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://on.muxihuayi.cn

TS:   s.split(",")
来源：http://ro.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ze.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pe.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://zq.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ks.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://is.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://lz.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://pv.colortex.cn

JS:   items.join(",")
来源：http://st.bjjhwx.cn

TS:   items.join(",")
来源：http://yn.hnjuh.cn

Java: String.join(",", items)
来源：http://lw.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://zf.wgjwhj.cn

Ruby: items.join(",")
来源：http://ub.wgjwhj.cn

C#:   string.Join(",", items)
来源：http://vh.huanxung.cn

[E09] 去除所有空白字符
来源：http://az.shxzskj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qa.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://od.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://tc.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://pk.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://mm.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gw.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xq.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tg.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://sy.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://py.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qv.521024.cn

JS:   "7".padStart(3, "0")
来源：http://yu.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://qf.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://vv.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jb.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mn.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://st.yuexingan06.cn

[E11] 反转字符串
来源：http://jb.shtwfgs.cn

Py:   s[::-1]
来源：http://ss.yuexingan06.cn

PHP:  strrev($s);
来源：http://av.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://ih.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://mt.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mm.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yp.gzmigu.cn

Ruby: s.reverse
来源：http://qt.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jr.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://hh.newstarts.cn

Py:   s.count("a")
来源：http://re.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://hy.9csxet.cn

JS:   s.split("a").length - 1
来源：http://jp.huanxung.cn

TS:   s.split("a").length - 1
来源：http://bl.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://um.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://nl.haigaiapp.cn

Ruby: s.count("a")
来源：http://yk.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://dp.szxytkj.cn

[E13] 逐字符遍历
来源：http://jp.colortex.cn

Py:   for ch in s: print(ch)
来源：http://ik.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zk.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://da.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wd.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rq.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://am.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hg.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ym.huanxung.cn

[E14] URL 编码与 Base64
来源：http://zf.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bo.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://us.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nm.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sg.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ut.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ym.muxihuayi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vs.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://df.szsharing.cn

[E15] HTML 转义 / 反转义
来源：http://ck.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xf.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rj.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://go.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ri.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wl.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ky.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ng.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qi.shtwfgs.cn

[E16] 数字千分位
来源：http://wr.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://pe.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://xb.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gu.521024.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yq.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oi.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tv.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bu.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://hu.gzmigu.cn

[E17] 首字母大写
来源：http://sm.chemitech.net.cn


<!-- 参考信息 -->