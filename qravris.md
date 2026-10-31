代发 wailian999

PHP:  sort($arr);
来源：http://kc.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cm.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ke.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cm.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hw.shtwfgs.cn

Ruby: arr.sort
来源：http://qr.521024.cn

C#:   list.Sort();
来源：http://mk.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ql.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ng.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yc.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kf.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rm.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://we.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bc.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ya.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gv.nszjky.cn

[D11] 反转数组
来源：http://cn.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://iv.newstarts.cn

PHP:  array_reverse($arr);
来源：http://cs.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bk.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://nm.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://wj.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://de.lnxyls.cn

Ruby: arr.reverse
来源：http://yd.chemitech.net.cn

C#:   list.Reverse();
来源：http://mu.yuexingan06.cn

[D12] 查找元素下标
来源：http://rb.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://dc.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mb.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tb.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gh.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xe.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://qp.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://sg.huanxung.cn

C#:   list.IndexOf(x);
来源：http://xb.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://dx.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ct.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hq.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://ek.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://ih.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://or.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xh.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gu.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gz.newstarts.cn

[D14] 映射转换（每个元素变形）
来源：http://hb.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://it.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ph.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://rt.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://rm.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qm.szxytkj.cn

Go:   // 手写循环
来源：http://px.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sx.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://is.muxihuayi.cn

[D15] 去重
来源：http://yr.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gq.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://dt.asd995.cn

JS:   [...new Set(arr)]
来源：http://gi.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://ku.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dr.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wk.huanxung.cn

Ruby: arr.uniq
来源：http://ff.521024.cn

C#:   list.Distinct().ToList()
来源：http://du.jctech888.com.cn

[D16] 求和与平均值
来源：http://bq.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tm.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hp.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jt.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yt.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jd.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://nr.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://el.521024.cn

C#:   list.Sum();  list.Average()
来源：http://uv.9csxet.cn

[D17] 最大值与最小值
来源：http://ol.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://xj.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://ty.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gh.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://hl.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mk.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nu.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://wq.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://gh.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://xp.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yb.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://gg.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dp.szxytkj.cn

TS:   nested.flat();
来源：http://yt.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ty.hnjuh.cn

Go:   // 手写双层循环
来源：http://lg.panjiajie.cn

Ruby: nested.flatten
来源：http://xa.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bh.lnxyls.cn

[D19] 按字段分组
来源：http://fl.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jp.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gz.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://er.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sk.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ef.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://yh.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://co.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wi.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://ej.huixiangedu.cn

Py:   Counter(arr)
来源：http://hc.newstarts.cn

PHP:  array_count_values($arr);
来源：http://pz.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xe.huixinmuqiang.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yd.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fu.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://mg.jctech888.com.cn

Ruby: arr.tally
来源：http://fb.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://td.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://pr.521024.cn

Py:   x in arr
来源：http://gj.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://qi.huixiangedu.cn

JS:   arr.includes(x)
来源：http://ft.nszjky.cn

TS:   arr.includes(x)
来源：http://yh.chemitech.net.cn

Java: list.contains(x)
来源：http://nf.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://lj.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://ym.huixiangedu.cn

C#:   list.Contains(x)
来源：http://pg.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://wj.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wg.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fk.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ra.nszjky.cn

TS:   [...arr];
来源：http://fm.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://la.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wi.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://ra.muxihuayi.cn

C#:   new List<int>(list);
来源：http://kp.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://hf.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yf.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://se.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jf.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sx.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hx.lnxyls.cn

Go:   // 手写循环
来源：http://xk.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pb.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ht.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://ym.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pw.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://si.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://od.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hy.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kv.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://to.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ob.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ta.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://eu.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ib.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://he.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cb.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qx.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pv.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qa.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ei.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xp.huixiangedu.cn

[D26] 数组转字符串
来源：http://pc.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://tf.asd995.cn

PHP:  implode(", ", $arr);
来源：http://qe.jctech888.com.cn

JS:   arr.join(", ")
来源：http://dm.shxzukj.cn

TS:   arr.join(", ")
来源：http://by.jctech888.com.cn

Java: String.join(", ", list)
来源：http://ng.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://pn.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://mj.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://cx.9csxet.cn

================================================================================
来源：http://xo.bookmarksfly.cn

E. 字符串处理
来源：http://nz.asd995.cn

================================================================================
来源：http://rt.bjjhwx.cn

[E01] 拼接字符串
来源：http://mx.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ru.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nv.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qu.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cz.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://at.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ml.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gb.haigaiapp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kc.nicolike.cn

[E02] 重复字符串
来源：http://xk.wgjwhj.cn

Py:   "ab" * 3
来源：http://qk.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://mq.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://gc.newstarts.cn

TS:   "ab".repeat(3)
来源：http://zc.szsharing.cn

Java: "ab".repeat(3)
来源：http://yo.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://pe.9csxet.cn

Ruby: "ab" * 3
来源：http://ll.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vo.szxytkj.cn

[E03] 截取子串
来源：http://pv.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cz.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ls.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dv.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://se.huixinmuqiang.cn

Java: s.substring(1, 4)
来源：http://ek.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jp.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ja.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://zf.shxzukj.cn

[E04] 查找子串位置
来源：http://zq.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://sh.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://ua.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tf.shxzukj.cn

TS:   s.indexOf("x")
来源：http://zw.shtwfgs.cn

Java: s.indexOf("x")
来源：http://ms.chemitech.net.cn

Go:   strings.Index(s, "x")
来源：http://iy.shxzskj.cn

Ruby: s.index("x")
来源：http://th.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://fc.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://or.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qo.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fs.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hn.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mm.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dq.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jt.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nh.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mb.asd995.cn

[E06] 替换子串
来源：http://mh.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qt.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://yv.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tr.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://er.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zn.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qr.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xu.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://sg.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://ku.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nu.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ka.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oq.colortex.cn

TS:   s.split(",")
来源：http://cw.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://re.panjiajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ow.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://id.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ex.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://qx.newstarts.cn

Py:   ",".join(items)
来源：http://wn.szsharing.cn

PHP:  implode(",", $items);
来源：http://fg.lnxyls.cn

JS:   items.join(",")
来源：http://wv.nicolike.cn

TS:   items.join(",")
来源：http://rp.gzmigu.cn

Java: String.join(",", items)
来源：http://jf.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://rz.9csxet.cn

Ruby: items.join(",")
来源：http://fm.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://um.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://cd.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lo.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wv.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://gn.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://fg.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://em.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vt.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yi.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eb.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://or.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sb.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gs.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://xq.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://lo.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://pl.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wy.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mb.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ey.gzmigu.cn

[E11] 反转字符串
来源：http://ol.521024.cn

Py:   s[::-1]
来源：http://lc.haigaiapp.cn

PHP:  strrev($s);
来源：http://ks.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://hw.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://vr.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xt.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ju.gzmigu.cn

Ruby: s.reverse
来源：http://jl.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://aw.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://gu.hnjuh.cn

Py:   s.count("a")
来源：http://yn.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://qu.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://vp.nicolike.cn

TS:   s.split("a").length - 1
来源：http://gw.colortex.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ro.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://yk.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://vp.shtwfgs.cn

C#:   s.Count(c => c == 'a')
来源：http://tu.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://mw.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://ir.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xh.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qd.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qi.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hw.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zw.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sp.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wr.nicolike.cn

[E14] URL 编码与 Base64
来源：http://uv.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ih.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ui.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nu.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qq.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://by.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://of.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ny.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mw.521024.cn

[E15] HTML 转义 / 反转义
来源：http://ii.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://oi.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tr.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eo.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sx.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ij.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cw.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://li.jianghongdianzi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fx.huixiangedu.cn

[E16] 数字千分位
来源：http://ot.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://qt.huixinmuqiang.cn


<!-- 参考信息 -->