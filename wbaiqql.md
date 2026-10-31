代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fz.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fh.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lv.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qk.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kb.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jl.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wz.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wc.lnxyls.cn

[D11] 反转数组
来源：http://sb.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sl.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://qk.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vk.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://bd.hnjuh.cn

Java: Collections.reverse(list);
来源：http://ai.521024.cn

Go:   slices.Reverse(arr)
来源：http://nn.hnjuh.cn

Ruby: arr.reverse
来源：http://ai.shxzskj.cn

C#:   list.Reverse();
来源：http://ju.521024.cn

[D12] 查找元素下标
来源：http://rv.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://qe.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vk.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sx.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tt.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eg.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://wr.wgjwhj.cn

Ruby: arr.index(x)
来源：http://go.521024.cn

C#:   list.IndexOf(x);
来源：http://nx.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://wl.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tm.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fl.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://kg.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://sg.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qy.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bq.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wz.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rh.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://df.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ku.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vb.521024.cn

JS:   arr.map(x => x * 2)
来源：http://fk.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://vf.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qi.szsharing.cn

Go:   // 手写循环
来源：http://hk.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://so.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ny.asd995.cn

[D15] 去重
来源：http://er.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fo.colortex.cn

PHP:  array_unique($arr);
来源：http://qs.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://nq.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://fe.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fg.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://la.shtwfgs.cn

Ruby: arr.uniq
来源：http://tz.521024.cn

C#:   list.Distinct().ToList()
来源：http://ah.hahajie.cn

[D16] 求和与平均值
来源：http://lz.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wj.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vm.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ps.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sj.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xw.nicolike.cn

Go:   // 手写循环累加
来源：http://qi.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wd.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://pp.asd995.cn

[D17] 最大值与最小值
来源：http://fx.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://jr.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://av.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yl.szxytkj.cn

TS:   Math.max(...arr);
来源：http://aa.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wo.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qi.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://un.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://ye.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://ld.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hk.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://xi.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zx.yuexingan06.cn

TS:   nested.flat();
来源：http://oe.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ir.lnxyls.cn

Go:   // 手写双层循环
来源：http://wr.shxzskj.cn

Ruby: nested.flatten
来源：http://oe.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yt.huixinmuqiang.cn

[D19] 按字段分组
来源：http://nd.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mu.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fr.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nt.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gf.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ss.521024.cn

Go:   // 手写 map[string][]T
来源：http://xa.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lp.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ya.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://ks.nicolike.cn

Py:   Counter(arr)
来源：http://aq.colortex.cn

PHP:  array_count_values($arr);
来源：http://xa.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://md.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ux.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oc.szsharing.cn

Go:   // 手写 map[T]int
来源：http://st.bjjhwx.cn

Ruby: arr.tally
来源：http://by.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qy.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://dd.hnjuh.cn

Py:   x in arr
来源：http://rv.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://nx.yuntaijiaju.cn

JS:   arr.includes(x)
来源：http://jd.nicolike.cn

TS:   arr.includes(x)
来源：http://in.gzmigu.cn

Java: list.contains(x)
来源：http://mq.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://zj.gzmigu.cn

Ruby: arr.include?(x)
来源：http://pb.szsharing.cn

C#:   list.Contains(x)
来源：http://ug.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://uk.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rg.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cm.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wf.bookmarksfly.cn

TS:   [...arr];
来源：http://nw.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://rf.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vw.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://bf.shxzukj.cn

C#:   new List<int>(list);
来源：http://ox.hahajie.cn

[D23] reduce 累积计算
来源：http://da.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yo.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ra.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dv.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://os.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ox.lnxyls.cn

Go:   // 手写循环
来源：http://mh.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yj.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uk.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://zg.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vi.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hd.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kh.shxzukj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bo.shxzukj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ib.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ti.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jp.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fy.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://wz.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hp.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hs.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hu.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cd.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://am.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xx.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fi.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xf.szxytkj.cn

[D26] 数组转字符串
来源：http://ij.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://rn.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://gh.nszjky.cn

JS:   arr.join(", ")
来源：http://ia.bjjhwx.cn

TS:   arr.join(", ")
来源：http://qw.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://qe.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://hc.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://oo.nszjky.cn

C#:   string.Join(", ", list)
来源：http://jm.asd995.cn

================================================================================
来源：http://ni.muxihuayi.cn

E. 字符串处理
来源：http://pz.9csxet.cn

================================================================================
来源：http://lj.nszjky.cn

[E01] 拼接字符串
来源：http://we.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wl.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vm.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cn.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yv.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dw.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ex.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://on.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zs.9csxet.cn

[E02] 重复字符串
来源：http://et.jctech888.com.cn

Py:   "ab" * 3
来源：http://xk.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://xp.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://bu.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://lg.nicolike.cn

Java: "ab".repeat(3)
来源：http://vl.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://yi.9csxet.cn

Ruby: "ab" * 3
来源：http://td.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wd.gzmigu.cn

[E03] 截取子串
来源：http://ho.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mp.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oc.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pb.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://xz.shxzukj.cn

Java: s.substring(1, 4)
来源：http://qv.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vx.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://um.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://dq.shtwfgs.cn

[E04] 查找子串位置
来源：http://rc.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://pf.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://aa.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fq.hnjuh.cn

TS:   s.indexOf("x")
来源：http://tf.szxytkj.cn

Java: s.indexOf("x")
来源：http://fz.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://tu.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://ju.hahajie.cn

C#:   s.IndexOf("x")
来源：http://ys.yuexingan06.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mp.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aa.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vv.yuexingan06.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gb.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wq.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yd.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qt.521024.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ry.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://na.jianghongdianzi.cn

[E06] 替换子串
来源：http://ps.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gz.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://ok.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jj.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://pv.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qd.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bs.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ln.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://yl.shxzskj.cn

[E07] 按分隔符拆分
来源：http://ao.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oq.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tb.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cx.huixinmuqiang.cn

TS:   s.split(",")
来源：http://yl.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hp.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lo.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://ro.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qi.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://uq.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://dq.huanxung.cn

PHP:  implode(",", $items);
来源：http://nf.panjiajie.cn

JS:   items.join(",")
来源：http://nj.521024.cn

TS:   items.join(",")
来源：http://rt.jctech888.com.cn

Java: String.join(",", items)
来源：http://zj.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://nu.shtwfgs.cn

Ruby: items.join(",")
来源：http://cx.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://hw.shxzukj.cn

[E09] 去除所有空白字符
来源：http://ja.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lj.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vd.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://fl.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://wr.nszjky.cn

Java: s.replaceAll("\\s+", "")
来源：http://yt.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bp.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nf.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ff.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://ek.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pd.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dw.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://ky.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://og.colortex.cn

Java: String.format("%03d", 7)
来源：http://qj.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mr.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dn.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ns.jianghongdianzi.cn

[E11] 反转字符串
来源：http://zw.lnxyls.cn

Py:   s[::-1]
来源：http://cn.nicolike.cn

PHP:  strrev($s);
来源：http://hc.colortex.cn

JS:   [...s].reverse().join("")
来源：http://fj.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://cd.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jh.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gg.yuntaijiaju.cn

Ruby: s.reverse
来源：http://la.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://eq.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://ls.wgjwhj.cn

Py:   s.count("a")
来源：http://xj.wgjwhj.cn

PHP:  substr_count($s, "a");
来源：http://tt.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://mi.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://pt.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tz.asd995.cn

Go:   strings.Count(s, "a")
来源：http://wo.szxytkj.cn

Ruby: s.count("a")
来源：http://vx.shtwfgs.cn

C#:   s.Count(c => c == 'a')
来源：http://mk.hahajie.cn

[E13] 逐字符遍历
来源：http://yu.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://cw.nicolike.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vv.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cg.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ml.haigaiapp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fp.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zv.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ut.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uj.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://lc.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mq.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kh.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oo.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tj.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ha.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xe.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zg.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pu.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://fc.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://so.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fu.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fz.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tp.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jd.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ut.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tt.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://my.haigaiapp.cn

[E16] 数字千分位
来源：http://su.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://cw.newstarts.cn

PHP:  number_format(1234567);
来源：http://sk.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rl.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lb.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bb.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dk.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xs.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://hm.yuntaijiaju.cn

[E17] 首字母大写
来源：http://sn.shxzskj.cn


<!-- 参考信息 -->