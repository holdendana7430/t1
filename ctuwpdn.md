代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://xp.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://tc.jctech888.com.cn

[D09] 排序（升序）
来源：http://pd.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://yd.colortex.cn

PHP:  sort($arr);
来源：http://cs.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nm.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bk.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gv.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ut.panjiajie.cn

Ruby: arr.sort
来源：http://tj.9csxet.cn

C#:   list.Sort();
来源：http://wb.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://of.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jh.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qo.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gw.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://os.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dx.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fe.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uk.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xb.szsharing.cn

[D11] 反转数组
来源：http://yf.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://by.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://xy.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oe.shxzukj.cn

TS:   [...arr].reverse();
来源：http://sq.9csxet.cn

Java: Collections.reverse(list);
来源：http://cc.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://it.chemitech.net.cn

Ruby: arr.reverse
来源：http://cp.asd995.cn

C#:   list.Reverse();
来源：http://jd.jctech888.com.cn

[D12] 查找元素下标
来源：http://or.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://gm.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hh.shxzskj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mc.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ez.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yf.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://iv.chemitech.net.cn

Ruby: arr.index(x)
来源：http://md.colortex.cn

C#:   list.IndexOf(x);
来源：http://lo.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://uv.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ul.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tb.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://jw.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://lo.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ae.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://er.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bf.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://km.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://oo.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ye.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ab.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://ks.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://xh.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sn.521024.cn

Go:   // 手写循环
来源：http://xg.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wc.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gi.jctech888.com.cn

[D15] 去重
来源：http://tl.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mo.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://es.521024.cn

JS:   [...new Set(arr)]
来源：http://cj.szsharing.cn

TS:   [...new Set(arr)]
来源：http://pv.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uv.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xo.colortex.cn

Ruby: arr.uniq
来源：http://qx.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://ou.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://sg.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xw.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qo.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ul.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bq.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gq.521024.cn

Go:   // 手写循环累加
来源：http://yk.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ae.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://hk.yuexingan06.cn

[D17] 最大值与最小值
来源：http://bn.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://vy.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://vl.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ov.szsharing.cn

TS:   Math.max(...arr);
来源：http://nc.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dz.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bs.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://qc.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://ef.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://rq.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mg.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://hz.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qp.haigaiapp.cn

TS:   nested.flat();
来源：http://yp.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zm.lnxyls.cn

Go:   // 手写双层循环
来源：http://cs.jctech888.com.cn

Ruby: nested.flatten
来源：http://vz.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wl.shxzskj.cn

[D19] 按字段分组
来源：http://ht.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kz.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jp.colortex.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pu.gzmigu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qn.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://je.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://hw.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fb.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fn.colortex.cn

[D20] 统计每个元素出现次数
来源：http://ln.521024.cn

Py:   Counter(arr)
来源：http://yp.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://lo.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ie.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tv.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ea.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://un.hahajie.cn

Ruby: arr.tally
来源：http://ix.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yz.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://kw.colortex.cn

Py:   x in arr
来源：http://eo.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://pw.wgjwhj.cn

JS:   arr.includes(x)
来源：http://sb.hnjuh.cn

TS:   arr.includes(x)
来源：http://kp.muxihuayi.cn

Java: list.contains(x)
来源：http://kr.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://as.szsharing.cn

Ruby: arr.include?(x)
来源：http://cy.nszjky.cn

C#:   list.Contains(x)
来源：http://qo.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://fr.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xy.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mt.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eb.chemitech.net.cn

TS:   [...arr];
来源：http://wv.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://le.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ej.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://vb.521024.cn

C#:   new List<int>(list);
来源：http://bi.bjjhwx.cn

[D23] reduce 累积计算
来源：http://lz.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bo.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zv.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fo.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nt.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bp.jctech888.com.cn

Go:   // 手写循环
来源：http://kt.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fp.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cr.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://ap.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pi.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dg.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uu.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://is.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yt.9csxet.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://we.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ci.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ox.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://uf.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xj.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rd.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jl.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://di.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cf.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://un.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ne.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mc.szxytkj.cn

[D26] 数组转字符串
来源：http://ya.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://xa.asd995.cn

PHP:  implode(", ", $arr);
来源：http://xm.huixiangedu.cn

JS:   arr.join(", ")
来源：http://rn.asd995.cn

TS:   arr.join(", ")
来源：http://wq.huixiangedu.cn

Java: String.join(", ", list)
来源：http://ih.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://gx.nszjky.cn

Ruby: arr.join(", ")
来源：http://vk.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://gq.asd995.cn

================================================================================
来源：http://xf.huanxung.cn

E. 字符串处理
来源：http://ff.gzmigu.cn

================================================================================
来源：http://dt.lnxyls.cn

[E01] 拼接字符串
来源：http://fa.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ss.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vv.szsharing.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hv.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wo.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ai.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sg.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ks.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nm.lnxyls.cn

[E02] 重复字符串
来源：http://th.muxihuayi.cn

Py:   "ab" * 3
来源：http://ce.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://bu.521024.cn

JS:   "ab".repeat(3)
来源：http://nt.panjiajie.cn

TS:   "ab".repeat(3)
来源：http://pm.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://xw.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://qc.szxytkj.cn

Ruby: "ab" * 3
来源：http://mw.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yp.haigaiapp.cn

[E03] 截取子串
来源：http://yt.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cw.panjiajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rw.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://il.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://gy.panjiajie.cn

Java: s.substring(1, 4)
来源：http://qn.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qm.panjiajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pp.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://zt.szxytkj.cn

[E04] 查找子串位置
来源：http://nl.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://uh.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://yn.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pg.nicolike.cn

TS:   s.indexOf("x")
来源：http://gl.wgjwhj.cn

Java: s.indexOf("x")
来源：http://tj.huixiangedu.cn

Go:   strings.Index(s, "x")
来源：http://gl.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://xx.hahajie.cn

C#:   s.IndexOf("x")
来源：http://la.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ht.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lw.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oh.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://al.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ru.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eq.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ui.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zq.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ub.shxzskj.cn

[E06] 替换子串
来源：http://uv.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vo.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://kk.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jz.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://nc.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zf.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pd.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://id.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://bv.hnjuh.cn

[E07] 按分隔符拆分
来源：http://bf.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ks.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rr.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hf.jianghongdianzi.cn

TS:   s.split(",")
来源：http://ka.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kh.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uz.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://ud.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ph.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://wl.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://mi.shxzukj.cn

PHP:  implode(",", $items);
来源：http://ym.hnjuh.cn

JS:   items.join(",")
来源：http://dn.szxytkj.cn

TS:   items.join(",")
来源：http://az.jctech888.com.cn

Java: String.join(",", items)
来源：http://gl.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://fq.huanxung.cn

Ruby: items.join(",")
来源：http://am.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://nh.hnjuh.cn

[E09] 去除所有空白字符
来源：http://wh.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rx.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vl.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://cz.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://fb.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://ms.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://on.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ru.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://as.yuntaijiaju.cn

[E10] 左侧补零 / 定长填充
来源：http://kl.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fm.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bc.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://sh.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://ya.colortex.cn

Java: String.format("%03d", 7)
来源：http://rw.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xt.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yj.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ir.huanxung.cn

[E11] 反转字符串
来源：http://jo.shxzukj.cn

Py:   s[::-1]
来源：http://zl.newstarts.cn

PHP:  strrev($s);
来源：http://rn.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://ju.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://wv.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cp.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://eu.jctech888.com.cn

Ruby: s.reverse
来源：http://fp.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://es.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://oa.nicolike.cn

Py:   s.count("a")
来源：http://ms.asd995.cn

PHP:  substr_count($s, "a");
来源：http://up.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://tt.521024.cn

TS:   s.split("a").length - 1
来源：http://zf.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zx.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://ff.nszjky.cn

Ruby: s.count("a")
来源：http://nr.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://fl.newstarts.cn

[E13] 逐字符遍历
来源：http://ku.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://qe.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sx.huixiangedu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jx.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xl.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ra.colortex.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ik.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vo.haigaiapp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ue.colortex.cn

[E14] URL 编码与 Base64
来源：http://nk.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fe.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://so.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mk.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cn.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ac.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ym.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://im.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ed.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://aq.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xy.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sn.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zi.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yf.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vx.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fi.szsharing.cn


<!-- 参考信息 -->