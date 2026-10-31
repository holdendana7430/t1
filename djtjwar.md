代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fm.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uo.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ep.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gt.yuexingan06.cn

[D11] 反转数组
来源：http://es.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://it.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://wu.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vs.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://hv.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://uq.asd995.cn

Go:   slices.Reverse(arr)
来源：http://dd.colortex.cn

Ruby: arr.reverse
来源：http://vd.asd995.cn

C#:   list.Reverse();
来源：http://fy.szxytkj.cn

[D12] 查找元素下标
来源：http://ex.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://ak.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://at.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wv.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rr.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qv.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://qv.gzmigu.cn

Ruby: arr.index(x)
来源：http://ga.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://ui.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://yq.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uu.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qh.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://rn.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://it.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rg.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uv.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xj.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qm.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://rn.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vy.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zr.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://yk.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://tx.huixinmuqiang.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mo.shtwfgs.cn

Go:   // 手写循环
来源：http://df.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fg.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bt.gzmigu.cn

[D15] 去重
来源：http://ss.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nf.colortex.cn

PHP:  array_unique($arr);
来源：http://hn.nszjky.cn

JS:   [...new Set(arr)]
来源：http://km.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://cd.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gn.chemitech.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qg.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://zw.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://gb.muxihuayi.cn

[D16] 求和与平均值
来源：http://cn.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nh.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nd.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dw.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fj.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mh.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://da.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uv.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://on.gzmigu.cn

[D17] 最大值与最小值
来源：http://df.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://zs.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://iz.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zz.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://vn.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cp.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ry.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://nm.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://iu.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://tu.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fh.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://oh.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cl.yuntaijiaju.cn

TS:   nested.flat();
来源：http://fb.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ek.muxihuayi.cn

Go:   // 手写双层循环
来源：http://rr.newstarts.cn

Ruby: nested.flatten
来源：http://xb.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nr.jianghongdianzi.cn

[D19] 按字段分组
来源：http://xf.bjjhwx.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sx.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hl.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ot.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xl.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qq.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://mn.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mq.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wd.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://lf.hnjuh.cn

Py:   Counter(arr)
来源：http://pa.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://ae.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iz.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cy.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wd.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://ab.asd995.cn

Ruby: arr.tally
来源：http://jb.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yc.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://pi.nicolike.cn

Py:   x in arr
来源：http://ru.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://ej.hnjuh.cn

JS:   arr.includes(x)
来源：http://wu.chemitech.net.cn

TS:   arr.includes(x)
来源：http://pn.colortex.cn

Java: list.contains(x)
来源：http://on.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://kr.9csxet.cn

Ruby: arr.include?(x)
来源：http://cu.shxzskj.cn

C#:   list.Contains(x)
来源：http://cx.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://na.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qt.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iu.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pu.hahajie.cn

TS:   [...arr];
来源：http://yt.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://ms.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cx.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://dj.muxihuayi.cn

C#:   new List<int>(list);
来源：http://po.muxihuayi.cn

[D23] reduce 累积计算
来源：http://me.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gf.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rx.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pq.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bp.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wf.wgjwhj.cn

Go:   // 手写循环
来源：http://jt.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vn.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xz.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://mw.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://by.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://he.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yj.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sl.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fn.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gr.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bc.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fn.bjjhwx.cn

[D25] Set 集合去重与交并差
来源：http://hi.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ts.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bs.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ro.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ka.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kz.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gw.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://og.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://te.jctech888.com.cn

[D26] 数组转字符串
来源：http://vv.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://je.asd995.cn

PHP:  implode(", ", $arr);
来源：http://dy.shxzskj.cn

JS:   arr.join(", ")
来源：http://gt.nszjky.cn

TS:   arr.join(", ")
来源：http://dq.szsharing.cn

Java: String.join(", ", list)
来源：http://uj.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://gf.hnjuh.cn

Ruby: arr.join(", ")
来源：http://gr.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://ne.chemitech.net.cn

================================================================================
来源：http://td.shxzukj.cn

E. 字符串处理
来源：http://zs.nszjky.cn

================================================================================
来源：http://qa.hnjuh.cn

[E01] 拼接字符串
来源：http://nx.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lq.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cf.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rm.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gg.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qk.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pr.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mg.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rk.wgjwhj.cn

[E02] 重复字符串
来源：http://zv.521024.cn

Py:   "ab" * 3
来源：http://zw.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://dg.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://fe.panjiajie.cn

TS:   "ab".repeat(3)
来源：http://og.gzmigu.cn

Java: "ab".repeat(3)
来源：http://nu.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://lx.haigaiapp.cn

Ruby: "ab" * 3
来源：http://xe.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://as.bookmarksfly.cn

[E03] 截取子串
来源：http://oe.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sj.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vp.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://df.szsharing.cn

TS:   s.slice(1, 4)
来源：http://jw.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://qy.nszjky.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ra.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://av.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://ju.huixiangedu.cn

[E04] 查找子串位置
来源：http://qj.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://pi.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://tb.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xz.szsharing.cn

TS:   s.indexOf("x")
来源：http://zl.nicolike.cn

Java: s.indexOf("x")
来源：http://rb.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://sf.yuexingan06.cn

Ruby: s.index("x")
来源：http://le.szsharing.cn

C#:   s.IndexOf("x")
来源：http://cz.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://of.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rd.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ql.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wq.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jn.wgjwhj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ma.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://om.nicolike.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://br.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iu.haigaiapp.cn

[E06] 替换子串
来源：http://wb.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qq.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://pr.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ec.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://cv.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uk.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hu.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wz.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://dz.hnjuh.cn

[E07] 按分隔符拆分
来源：http://lf.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zh.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hk.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dm.asd995.cn

TS:   s.split(",")
来源：http://ju.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uj.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kn.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://pl.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ei.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://qk.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://mc.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://sv.bjjhwx.cn

JS:   items.join(",")
来源：http://si.nicolike.cn

TS:   items.join(",")
来源：http://vh.asd995.cn

Java: String.join(",", items)
来源：http://ee.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://ko.haigaiapp.cn

Ruby: items.join(",")
来源：http://bs.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://zx.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://ec.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bw.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tr.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://mr.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://rl.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://bs.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lq.huixinmuqiang.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vp.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uo.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://tm.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hc.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kq.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://ln.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://es.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://kj.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wy.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sb.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ei.9csxet.cn

[E11] 反转字符串
来源：http://py.bookmarksfly.cn

Py:   s[::-1]
来源：http://dl.panjiajie.cn

PHP:  strrev($s);
来源：http://wi.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://ig.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://pi.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ab.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zr.chemitech.net.cn

Ruby: s.reverse
来源：http://nc.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ji.521024.cn

[E12] 统计某字符出现次数
来源：http://pg.szsharing.cn

Py:   s.count("a")
来源：http://sa.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://fi.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://bl.colortex.cn

TS:   s.split("a").length - 1
来源：http://lx.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ms.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://tl.nicolike.cn

Ruby: s.count("a")
来源：http://bg.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://te.panjiajie.cn

[E13] 逐字符遍历
来源：http://yo.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://ah.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uz.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ci.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yp.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gb.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gm.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hc.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tc.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://ek.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mh.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fg.hnjuh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xu.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nm.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yj.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pq.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xu.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vh.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://gh.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zl.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mq.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bc.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ez.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vr.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tt.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ci.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xi.yuexingan06.cn

[E16] 数字千分位
来源：http://ci.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://mn.wgjwhj.cn

PHP:  number_format(1234567);
来源：http://ve.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xq.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ue.huanxung.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nz.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zh.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://av.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://kb.jianghongdianzi.cn

[E17] 首字母大写
来源：http://sd.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://km.hnjuh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xh.521024.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wb.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ek.huixiangedu.cn


<!-- 参考信息 -->