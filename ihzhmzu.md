代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ym.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wm.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xa.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://og.nicolike.cn

[D11] 反转数组
来源：http://ba.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dw.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://oi.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qw.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://xx.asd995.cn

Java: Collections.reverse(list);
来源：http://jo.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://jt.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://ud.yuexingan06.cn

C#:   list.Reverse();
来源：http://wm.nicolike.cn

[D12] 查找元素下标
来源：http://fu.521024.cn

Py:   arr.index(x);  x in arr
来源：http://rd.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zn.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mj.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fw.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jg.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://xq.yuntaijiaju.cn

Ruby: arr.index(x)
来源：http://iv.521024.cn

C#:   list.IndexOf(x);
来源：http://ks.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://hn.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ae.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gc.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://hl.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://dr.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bm.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ns.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cn.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://aa.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://zh.bjjhwx.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lu.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xr.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://ia.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://uj.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mb.yuntaijiaju.cn

Go:   // 手写循环
来源：http://gw.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rc.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://oz.hnjuh.cn

[D15] 去重
来源：http://xn.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wb.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://co.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://bj.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://wm.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ju.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vb.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://ih.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://lz.9csxet.cn

[D16] 求和与平均值
来源：http://xp.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eo.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qt.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pw.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tg.wgjwhj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yp.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://iq.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qf.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://ck.lnxyls.cn

[D17] 最大值与最小值
来源：http://nt.521024.cn

Py:   max(arr);  min(arr)
来源：http://tt.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://jq.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mu.nszjky.cn

TS:   Math.max(...arr);
来源：http://sq.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xn.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ii.colortex.cn

Ruby: arr.max;  arr.min
来源：http://fi.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://nt.asd995.cn

[D18] 扁平化嵌套数组
来源：http://mw.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://au.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://lv.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ax.jctech888.com.cn

TS:   nested.flat();
来源：http://oz.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gn.szsharing.cn

Go:   // 手写双层循环
来源：http://de.huixiangedu.cn

Ruby: nested.flatten
来源：http://if.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://iu.newstarts.cn

[D19] 按字段分组
来源：http://tz.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xn.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ve.lnxyls.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hy.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xt.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://or.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://sp.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yw.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rg.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://tf.nszjky.cn

Py:   Counter(arr)
来源：http://sz.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://vu.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pe.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sg.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ts.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://tv.bjjhwx.cn

Ruby: arr.tally
来源：http://pq.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ou.colortex.cn

[D21] 判断是否包含某元素
来源：http://iz.bookmarksfly.cn

Py:   x in arr
来源：http://ud.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://sg.szsharing.cn

JS:   arr.includes(x)
来源：http://ej.newstarts.cn

TS:   arr.includes(x)
来源：http://hq.hnjuh.cn

Java: list.contains(x)
来源：http://uz.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://bv.lnxyls.cn

Ruby: arr.include?(x)
来源：http://qt.muxihuayi.cn

C#:   list.Contains(x)
来源：http://nf.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://tl.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ts.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vr.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://st.yuntaijiaju.cn

TS:   [...arr];
来源：http://xn.szsharing.cn

Java: new ArrayList<>(list);
来源：http://jr.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://od.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://hs.szsharing.cn

C#:   new List<int>(list);
来源：http://ao.bjjhwx.cn

[D23] reduce 累积计算
来源：http://zg.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sr.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jo.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zm.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://if.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xd.lnxyls.cn

Go:   // 手写循环
来源：http://ja.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ha.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dz.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://xo.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://de.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://we.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tf.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ei.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ye.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jx.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qp.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aw.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://bi.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pn.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sq.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://al.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gh.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ob.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://av.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yk.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zv.shtwfgs.cn

[D26] 数组转字符串
来源：http://cc.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://hj.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://iq.haigaiapp.cn

JS:   arr.join(", ")
来源：http://pw.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://lt.lnxyls.cn

Java: String.join(", ", list)
来源：http://px.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://iz.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://te.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://ry.yuexingan06.cn

================================================================================
来源：http://tn.bjjhwx.cn

E. 字符串处理
来源：http://af.szxytkj.cn

================================================================================
来源：http://ba.chemitech.net.cn

[E01] 拼接字符串
来源：http://ui.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jt.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nq.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bm.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tq.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sw.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://so.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cu.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ql.colortex.cn

[E02] 重复字符串
来源：http://gb.bookmarksfly.cn

Py:   "ab" * 3
来源：http://ms.wgjwhj.cn

PHP:  str_repeat("ab", 3);
来源：http://ei.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://mv.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://op.szxytkj.cn

Java: "ab".repeat(3)
来源：http://zo.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://le.gzmigu.cn

Ruby: "ab" * 3
来源：http://ab.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cv.huixinmuqiang.cn

[E03] 截取子串
来源：http://bf.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nl.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xw.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jy.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://at.hnjuh.cn

Java: s.substring(1, 4)
来源：http://gi.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://or.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gr.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://pq.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://fi.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://wm.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://ob.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eg.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://wn.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://yf.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://wf.szsharing.cn

Ruby: s.index("x")
来源：http://qx.nicolike.cn

C#:   s.IndexOf("x")
来源：http://eb.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zb.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fw.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://at.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mk.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ys.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zl.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zg.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nn.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hp.chemitech.net.cn

[E06] 替换子串
来源：http://ne.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jm.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://jm.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sy.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://rf.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xw.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://et.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xp.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://bo.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://cj.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zs.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jn.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rc.lnxyls.cn

TS:   s.split(",")
来源：http://dq.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fh.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tn.asd995.cn

Ruby: s.split(",");  s.split
来源：http://ug.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ln.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://mg.bjjhwx.cn

Py:   ",".join(items)
来源：http://ox.asd995.cn

PHP:  implode(",", $items);
来源：http://qm.hahajie.cn

JS:   items.join(",")
来源：http://wk.bookmarksfly.cn

TS:   items.join(",")
来源：http://oo.nszjky.cn

Java: String.join(",", items)
来源：http://sn.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://fm.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://rc.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://xo.hnjuh.cn

[E09] 去除所有空白字符
来源：http://xe.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ms.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ax.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://kg.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://qi.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://yt.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ou.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xv.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uh.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://ll.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oh.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://te.newstarts.cn

JS:   "7".padStart(3, "0")
来源：http://ed.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://nr.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://ov.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ib.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vs.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bo.wgjwhj.cn

[E11] 反转字符串
来源：http://ig.9csxet.cn

Py:   s[::-1]
来源：http://jc.colortex.cn

PHP:  strrev($s);
来源：http://ks.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://vx.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://uc.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lw.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dg.muxihuayi.cn

Ruby: s.reverse
来源：http://ne.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wi.nszjky.cn

[E12] 统计某字符出现次数
来源：http://jf.panjiajie.cn

Py:   s.count("a")
来源：http://uz.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://nr.asd995.cn

JS:   s.split("a").length - 1
来源：http://xy.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://ih.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jb.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://ev.lnxyls.cn

Ruby: s.count("a")
来源：http://kq.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://hi.huixiangedu.cn

[E13] 逐字符遍历
来源：http://wr.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://oy.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xt.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lv.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ct.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ex.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aq.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gr.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yt.nszjky.cn

[E14] URL 编码与 Base64
来源：http://jv.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lh.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uw.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bx.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ic.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qs.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tf.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mv.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vt.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://yb.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sq.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ax.jianghongdianzi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ou.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jw.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lm.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bv.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ww.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yd.lnxyls.cn

[E16] 数字千分位
来源：http://oi.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://xl.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://lt.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xg.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kg.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://li.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://om.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ty.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://il.nszjky.cn

[E17] 首字母大写
来源：http://yb.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ed.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rt.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pw.shxzskj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ue.colortex.cn


<!-- 参考信息 -->