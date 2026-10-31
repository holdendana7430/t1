代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nu.haigaiapp.cn

Ruby: arr.sort
来源：http://fe.521024.cn

C#:   list.Sort();
来源：http://lt.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://za.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tr.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sz.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kz.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://au.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dw.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://re.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ij.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://su.huanxung.cn

[D11] 反转数组
来源：http://re.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jj.521024.cn

PHP:  array_reverse($arr);
来源：http://ue.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ug.haigaiapp.cn

TS:   [...arr].reverse();
来源：http://yl.gzmigu.cn

Java: Collections.reverse(list);
来源：http://ou.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://aw.yuexingan06.cn

Ruby: arr.reverse
来源：http://kg.huanxung.cn

C#:   list.Reverse();
来源：http://jq.haigaiapp.cn

[D12] 查找元素下标
来源：http://rm.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://po.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vx.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wl.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://al.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ej.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://qs.szxytkj.cn

Ruby: arr.index(x)
来源：http://xy.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://eq.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://qn.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ow.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dr.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://bo.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://eq.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tv.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://af.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jn.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yb.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://ir.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ca.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ip.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://gj.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://xk.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nw.hahajie.cn

Go:   // 手写循环
来源：http://jw.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yd.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yc.hahajie.cn

[D15] 去重
来源：http://us.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nx.lnxyls.cn

PHP:  array_unique($arr);
来源：http://te.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://np.hahajie.cn

TS:   [...new Set(arr)]
来源：http://fr.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ob.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jm.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://hw.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://mt.panjiajie.cn

[D16] 求和与平均值
来源：http://sp.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ey.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ei.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nn.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aw.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yv.asd995.cn

Go:   // 手写循环累加
来源：http://my.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://la.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://az.jctech888.com.cn

[D17] 最大值与最小值
来源：http://al.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://ue.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://jg.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fk.szsharing.cn

TS:   Math.max(...arr);
来源：http://ih.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://we.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eo.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://in.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://qv.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://qd.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://je.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://dj.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bq.haigaiapp.cn

TS:   nested.flat();
来源：http://xw.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hb.jctech888.com.cn

Go:   // 手写双层循环
来源：http://fs.nszjky.cn

Ruby: nested.flatten
来源：http://wg.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://is.bjjhwx.cn

[D19] 按字段分组
来源：http://jq.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qk.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qa.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uh.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zc.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jc.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://rt.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gb.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wk.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://ga.bjjhwx.cn

Py:   Counter(arr)
来源：http://to.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://cp.muxihuayi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gf.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mc.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ss.huanxung.cn

Go:   // 手写 map[T]int
来源：http://pu.jianghongdianzi.cn

Ruby: arr.tally
来源：http://to.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lb.szsharing.cn

[D21] 判断是否包含某元素
来源：http://fa.huixiangedu.cn

Py:   x in arr
来源：http://cx.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://fq.nicolike.cn

JS:   arr.includes(x)
来源：http://ni.shxzskj.cn

TS:   arr.includes(x)
来源：http://qf.nszjky.cn

Java: list.contains(x)
来源：http://xx.haigaiapp.cn

Go:   slices.Contains(arr, x)
来源：http://ih.szsharing.cn

Ruby: arr.include?(x)
来源：http://ll.wgjwhj.cn

C#:   list.Contains(x)
来源：http://zl.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://za.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dt.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fm.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ni.wgjwhj.cn

TS:   [...arr];
来源：http://ec.newstarts.cn

Java: new ArrayList<>(list);
来源：http://zc.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rr.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://yb.9csxet.cn

C#:   new List<int>(list);
来源：http://ub.shxzskj.cn

[D23] reduce 累积计算
来源：http://gj.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://id.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dt.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gr.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hg.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lg.nszjky.cn

Go:   // 手写循环
来源：http://py.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bt.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hh.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://gs.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dw.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vd.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bn.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jh.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mw.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ct.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dk.colortex.cn

[D25] Set 集合去重与交并差
来源：http://zx.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ky.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nx.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iu.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pi.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tp.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ys.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uo.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pn.chemitech.net.cn

[D26] 数组转字符串
来源：http://vc.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://un.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://cb.shtwfgs.cn

JS:   arr.join(", ")
来源：http://cd.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://ol.haigaiapp.cn

Java: String.join(", ", list)
来源：http://ut.hahajie.cn

Go:   strings.Join(strs, ", ")
来源：http://kb.szxytkj.cn

Ruby: arr.join(", ")
来源：http://sr.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://uk.huanxung.cn

================================================================================
来源：http://xk.hnjuh.cn

E. 字符串处理
来源：http://vi.jianghongdianzi.cn

================================================================================
来源：http://fx.521024.cn

[E01] 拼接字符串
来源：http://ud.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ea.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://li.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pg.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qf.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wj.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dl.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ej.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nn.chemitech.net.cn

[E02] 重复字符串
来源：http://ra.shxzskj.cn

Py:   "ab" * 3
来源：http://fk.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://fq.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://er.huanxung.cn

TS:   "ab".repeat(3)
来源：http://yd.hnjuh.cn

Java: "ab".repeat(3)
来源：http://zl.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://qs.yuexingan06.cn

Ruby: "ab" * 3
来源：http://lg.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qf.chemitech.net.cn

[E03] 截取子串
来源：http://wi.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dk.hahajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ej.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hg.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://kl.nicolike.cn

Java: s.substring(1, 4)
来源：http://du.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://it.panjiajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kf.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://yf.gzmigu.cn

[E04] 查找子串位置
来源：http://dj.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://zg.bjjhwx.cn

PHP:  strpos($s, "x");
来源：http://fv.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gw.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://jz.chemitech.net.cn

Java: s.indexOf("x")
来源：http://ge.huixiangedu.cn

Go:   strings.Index(s, "x")
来源：http://sf.huixiangedu.cn

Ruby: s.index("x")
来源：http://sa.colortex.cn

C#:   s.IndexOf("x")
来源：http://dd.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uw.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gh.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vs.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iy.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uu.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oy.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lt.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ys.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://af.chemitech.net.cn

[E06] 替换子串
来源：http://ad.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://be.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://xl.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nd.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://ic.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kb.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ou.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iu.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://pc.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://mm.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xy.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mm.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dw.shxzukj.cn

TS:   s.split(",")
来源：http://vo.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ke.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hh.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://fb.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kv.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://mt.chemitech.net.cn

Py:   ",".join(items)
来源：http://uf.hnjuh.cn

PHP:  implode(",", $items);
来源：http://zr.hnjuh.cn

JS:   items.join(",")
来源：http://pk.yuexingan06.cn

TS:   items.join(",")
来源：http://kp.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://gz.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://tu.haigaiapp.cn

Ruby: items.join(",")
来源：http://me.szxytkj.cn

C#:   string.Join(",", items)
来源：http://qv.panjiajie.cn

[E09] 去除所有空白字符
来源：http://kh.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nc.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bp.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://iv.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://zi.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://sr.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mx.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zt.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bo.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://ak.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dd.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vx.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://hb.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://be.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://yz.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hx.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jd.yuexingan06.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oo.shxzskj.cn

[E11] 反转字符串
来源：http://hp.haigaiapp.cn

Py:   s[::-1]
来源：http://ks.szsharing.cn

PHP:  strrev($s);
来源：http://dz.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://nm.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://rk.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://el.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bq.lnxyls.cn

Ruby: s.reverse
来源：http://kw.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qp.huanxung.cn

[E12] 统计某字符出现次数
来源：http://bx.bookmarksfly.cn

Py:   s.count("a")
来源：http://lz.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://ek.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://qi.szsharing.cn

TS:   s.split("a").length - 1
来源：http://gq.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://et.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://rp.yuexingan06.cn

Ruby: s.count("a")
来源：http://ri.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://qc.haigaiapp.cn

[E13] 逐字符遍历
来源：http://bs.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://ot.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pk.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yf.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://oi.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cq.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nb.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mh.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nc.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://uq.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tr.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eu.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ib.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wd.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yt.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vi.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ik.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ru.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://jq.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lp.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uy.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ni.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hu.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kz.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fi.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ei.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gy.huixiangedu.cn

[E16] 数字千分位
来源：http://gl.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://zx.lnxyls.cn

PHP:  number_format(1234567);
来源：http://zh.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://to.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bu.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kl.hahajie.cn


<!-- 参考信息 -->