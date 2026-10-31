代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oe.gzmigu.cn

Ruby: arr.sort
来源：http://ue.jianghongdianzi.cn

C#:   list.Sort();
来源：http://mq.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dc.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cp.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ll.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uo.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://td.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://np.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://md.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pw.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qw.jianghongdianzi.cn

[D11] 反转数组
来源：http://ie.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nh.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://dg.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rn.asd995.cn

TS:   [...arr].reverse();
来源：http://rx.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://uz.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://ky.colortex.cn

Ruby: arr.reverse
来源：http://rr.jctech888.com.cn

C#:   list.Reverse();
来源：http://zr.muxihuayi.cn

[D12] 查找元素下标
来源：http://un.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://uh.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fi.nicolike.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gk.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vv.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://in.asd995.cn

Go:   slices.Index(arr, x)
来源：http://hg.hahajie.cn

Ruby: arr.index(x)
来源：http://yt.521024.cn

C#:   list.IndexOf(x);
来源：http://qb.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://yz.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qm.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ni.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://kr.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://xs.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ej.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rx.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uy.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tc.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://be.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qy.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ir.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://ko.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://by.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jf.huixiangedu.cn

Go:   // 手写循环
来源：http://ed.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bh.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vm.jianghongdianzi.cn

[D15] 去重
来源：http://aa.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tu.panjiajie.cn

PHP:  array_unique($arr);
来源：http://fd.hahajie.cn

JS:   [...new Set(arr)]
来源：http://rt.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://el.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ia.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jj.szsharing.cn

Ruby: arr.uniq
来源：http://lv.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://bu.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://pv.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ef.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ss.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gd.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uo.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dt.hahajie.cn

Go:   // 手写循环累加
来源：http://lw.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rv.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://tj.szsharing.cn

[D17] 最大值与最小值
来源：http://bz.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://xh.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://fo.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://de.lnxyls.cn

TS:   Math.max(...arr);
来源：http://ha.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yg.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ad.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://fs.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://xy.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://pj.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xb.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://jn.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pf.wgjwhj.cn

TS:   nested.flat();
来源：http://zf.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qu.shxzskj.cn

Go:   // 手写双层循环
来源：http://im.shxzukj.cn

Ruby: nested.flatten
来源：http://ik.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://es.huixiangedu.cn

[D19] 按字段分组
来源：http://dt.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zv.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wz.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ht.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ti.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bu.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://lv.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zb.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xz.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://tr.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://fw.521024.cn

PHP:  array_count_values($arr);
来源：http://gv.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ll.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bi.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yf.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://pr.yuexingan06.cn

Ruby: arr.tally
来源：http://gh.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://el.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://yi.bjjhwx.cn

Py:   x in arr
来源：http://eo.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://dq.huanxung.cn

JS:   arr.includes(x)
来源：http://ee.yuexingan06.cn

TS:   arr.includes(x)
来源：http://oc.jianghongdianzi.cn

Java: list.contains(x)
来源：http://lc.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://zz.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://rz.huanxung.cn

C#:   list.Contains(x)
来源：http://fw.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://ix.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fr.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xv.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nt.muxihuayi.cn

TS:   [...arr];
来源：http://aq.newstarts.cn

Java: new ArrayList<>(list);
来源：http://cr.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mg.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://sc.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://gz.shxzskj.cn

[D23] reduce 累积计算
来源：http://vj.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uo.yuexingan06.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wq.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ki.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rb.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dr.panjiajie.cn

Go:   // 手写循环
来源：http://oq.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rp.chemitech.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kt.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://jo.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pd.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wv.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ap.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uv.huanxung.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fz.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mp.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eo.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mp.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://jg.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dc.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hv.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ih.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yj.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xn.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cc.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xe.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mm.shxzskj.cn

[D26] 数组转字符串
来源：http://sf.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://yy.bookmarksfly.cn

PHP:  implode(", ", $arr);
来源：http://lp.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://ld.wgjwhj.cn

TS:   arr.join(", ")
来源：http://gt.yuexingan06.cn

Java: String.join(", ", list)
来源：http://lf.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://qb.newstarts.cn

Ruby: arr.join(", ")
来源：http://oq.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://tv.huixiangedu.cn

================================================================================
来源：http://fq.huixiangedu.cn

E. 字符串处理
来源：http://du.wgjwhj.cn

================================================================================
来源：http://le.wgjwhj.cn

[E01] 拼接字符串
来源：http://ww.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nr.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ap.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qr.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vs.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://or.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xa.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mm.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mq.521024.cn

[E02] 重复字符串
来源：http://zr.szsharing.cn

Py:   "ab" * 3
来源：http://kl.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://lv.huanxung.cn

JS:   "ab".repeat(3)
来源：http://ke.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://qh.szsharing.cn

Java: "ab".repeat(3)
来源：http://lz.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://nq.yuexingan06.cn

Ruby: "ab" * 3
来源：http://yo.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ev.huixinmuqiang.cn

[E03] 截取子串
来源：http://gm.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://di.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ge.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tr.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://un.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://ag.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fz.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ml.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://ng.bookmarksfly.cn

[E04] 查找子串位置
来源：http://na.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://xf.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://st.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ps.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://bu.jianghongdianzi.cn

Java: s.indexOf("x")
来源：http://pf.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://ns.yuexingan06.cn

Ruby: s.index("x")
来源：http://to.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://rv.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://da.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lk.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nq.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ou.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zn.yuntaijiaju.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://as.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vu.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://au.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ea.hnjuh.cn

[E06] 替换子串
来源：http://ao.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vu.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://hj.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wc.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://wp.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jq.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ip.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ox.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://un.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://hg.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xm.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://at.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qq.bjjhwx.cn

TS:   s.split(",")
来源：http://ad.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://eb.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hi.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://or.panjiajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jt.colortex.cn

[E08] 数组按分隔符合并
来源：http://la.colortex.cn

Py:   ",".join(items)
来源：http://im.bookmarksfly.cn

PHP:  implode(",", $items);
来源：http://lh.haigaiapp.cn

JS:   items.join(",")
来源：http://dw.yuexingan06.cn

TS:   items.join(",")
来源：http://of.huanxung.cn

Java: String.join(",", items)
来源：http://vk.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://yn.panjiajie.cn

Ruby: items.join(",")
来源：http://xa.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://pm.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://uf.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kw.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ve.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://oz.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://dg.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://pa.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sh.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zq.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bn.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://hg.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ry.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://go.newstarts.cn

JS:   "7".padStart(3, "0")
来源：http://qj.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://cs.9csxet.cn

Java: String.format("%03d", 7)
来源：http://jo.wgjwhj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tj.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ue.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vf.huixiangedu.cn

[E11] 反转字符串
来源：http://do.huixiangedu.cn

Py:   s[::-1]
来源：http://jh.shtwfgs.cn

PHP:  strrev($s);
来源：http://oz.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://dt.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://ef.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jw.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://me.9csxet.cn

Ruby: s.reverse
来源：http://ma.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ey.9csxet.cn

[E12] 统计某字符出现次数
来源：http://ie.nszjky.cn

Py:   s.count("a")
来源：http://xo.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://na.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://up.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://kb.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gr.521024.cn

Go:   strings.Count(s, "a")
来源：http://ys.huanxung.cn

Ruby: s.count("a")
来源：http://ub.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://kl.lnxyls.cn

[E13] 逐字符遍历
来源：http://ar.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://gt.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ga.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xt.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mh.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rx.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://se.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fb.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ah.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://bp.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gs.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://np.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xo.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uy.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sw.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rv.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tb.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ce.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://jn.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iu.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dr.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tg.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ux.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kp.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oy.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://om.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wd.lnxyls.cn

[E16] 数字千分位
来源：http://zh.hahajie.cn

Py:   f"{1234567:,}"
来源：http://kt.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://ao.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xf.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xn.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://og.gzmigu.cn


<!-- 参考信息 -->