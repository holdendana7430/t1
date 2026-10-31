代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bd.huixiangedu.cn

Ruby: arr.sort
来源：http://cb.hnjuh.cn

C#:   list.Sort();
来源：http://di.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nu.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ga.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mu.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hc.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://je.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qw.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iu.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://re.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sr.bookmarksfly.cn

[D11] 反转数组
来源：http://je.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mn.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://sm.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hl.szxytkj.cn

TS:   [...arr].reverse();
来源：http://nd.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://sk.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://ww.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://bc.chemitech.net.cn

C#:   list.Reverse();
来源：http://cz.bookmarksfly.cn

[D12] 查找元素下标
来源：http://sj.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://lj.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zo.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fb.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ep.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mw.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://me.szxytkj.cn

Ruby: arr.index(x)
来源：http://jb.colortex.cn

C#:   list.IndexOf(x);
来源：http://bp.huanxung.cn

[D13] 过滤（保留满足条件的）
来源：http://ob.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pi.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ja.wgjwhj.cn

JS:   arr.filter(x => x > 3)
来源：http://ug.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://pm.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vy.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qr.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ju.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hb.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://cf.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lk.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lb.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://ak.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://ud.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bu.shxzukj.cn

Go:   // 手写循环
来源：http://wf.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rm.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mt.bjjhwx.cn

[D15] 去重
来源：http://km.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://af.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://hs.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://ro.szsharing.cn

TS:   [...new Set(arr)]
来源：http://on.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nd.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bh.521024.cn

Ruby: arr.uniq
来源：http://fv.521024.cn

C#:   list.Distinct().ToList()
来源：http://kh.9csxet.cn

[D16] 求和与平均值
来源：http://mp.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nt.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://si.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ny.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xz.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ze.haigaiapp.cn

Go:   // 手写循环累加
来源：http://hu.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ch.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://sd.yuexingan06.cn

[D17] 最大值与最小值
来源：http://bl.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://br.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://eb.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vk.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://fx.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gg.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nx.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://nf.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://ml.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://ee.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sq.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://qa.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yf.huixiangedu.cn

TS:   nested.flat();
来源：http://aq.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ts.nszjky.cn

Go:   // 手写双层循环
来源：http://fh.huanxung.cn

Ruby: nested.flatten
来源：http://ad.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rh.colortex.cn

[D19] 按字段分组
来源：http://to.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://me.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://du.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://at.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pj.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wv.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://xp.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rs.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pm.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://ok.huanxung.cn

Py:   Counter(arr)
来源：http://sc.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://pn.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jd.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vo.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qi.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://js.521024.cn

Ruby: arr.tally
来源：http://gw.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qm.szxytkj.cn

[D21] 判断是否包含某元素
来源：http://hp.hnjuh.cn

Py:   x in arr
来源：http://kl.huixiangedu.cn

PHP:  in_array($x, $arr, true);
来源：http://bg.huixiangedu.cn

JS:   arr.includes(x)
来源：http://xb.nicolike.cn

TS:   arr.includes(x)
来源：http://bm.gzmigu.cn

Java: list.contains(x)
来源：http://ia.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://ke.colortex.cn

Ruby: arr.include?(x)
来源：http://ry.jctech888.com.cn

C#:   list.Contains(x)
来源：http://rz.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://gh.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qr.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jg.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bv.wgjwhj.cn

TS:   [...arr];
来源：http://kf.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://pt.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xz.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://cr.bookmarksfly.cn

C#:   new List<int>(list);
来源：http://do.shtwfgs.cn

[D23] reduce 累积计算
来源：http://jv.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://np.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://io.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ca.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qg.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hh.asd995.cn

Go:   // 手写循环
来源：http://mq.muxihuayi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ky.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lj.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://xm.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://je.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mb.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fo.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pb.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ge.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qa.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mj.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fc.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://oa.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nn.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eu.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hk.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mv.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rg.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qy.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fv.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pz.hnjuh.cn

[D26] 数组转字符串
来源：http://df.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://yb.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://fh.hahajie.cn

JS:   arr.join(", ")
来源：http://op.hahajie.cn

TS:   arr.join(", ")
来源：http://ct.panjiajie.cn

Java: String.join(", ", list)
来源：http://tu.nicolike.cn

Go:   strings.Join(strs, ", ")
来源：http://ao.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://ja.huanxung.cn

C#:   string.Join(", ", list)
来源：http://gr.shxzskj.cn

================================================================================
来源：http://td.newstarts.cn

E. 字符串处理
来源：http://bt.huixinmuqiang.cn

================================================================================
来源：http://hb.gzmigu.cn

[E01] 拼接字符串
来源：http://lc.521024.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jd.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vz.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jq.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yb.521024.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ii.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pz.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sn.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gv.colortex.cn

[E02] 重复字符串
来源：http://pp.9csxet.cn

Py:   "ab" * 3
来源：http://tb.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://on.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://px.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://pt.szsharing.cn

Java: "ab".repeat(3)
来源：http://ej.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://aq.huixiangedu.cn

Ruby: "ab" * 3
来源：http://ug.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://in.panjiajie.cn

[E03] 截取子串
来源：http://ng.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gl.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pc.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lf.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://iv.9csxet.cn

Java: s.substring(1, 4)
来源：http://im.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ir.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mv.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://qt.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://sc.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://as.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://vm.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kh.huanxung.cn

TS:   s.indexOf("x")
来源：http://cq.jianghongdianzi.cn

Java: s.indexOf("x")
来源：http://fe.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://zg.yuexingan06.cn

Ruby: s.index("x")
来源：http://yy.shxzskj.cn

C#:   s.IndexOf("x")
来源：http://xo.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ct.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kv.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dn.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://le.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ii.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://el.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zk.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tw.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://km.gzmigu.cn

[E06] 替换子串
来源：http://ew.wgjwhj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jr.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://po.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oo.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://gm.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lp.yuntaijiaju.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zm.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rn.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://lx.521024.cn

[E07] 按分隔符拆分
来源：http://cd.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ck.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://li.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tp.muxihuayi.cn

TS:   s.split(",")
来源：http://mg.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ha.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pb.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://pt.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hm.hahajie.cn

[E08] 数组按分隔符合并
来源：http://qv.asd995.cn

Py:   ",".join(items)
来源：http://xw.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://pn.nicolike.cn

JS:   items.join(",")
来源：http://gl.hnjuh.cn

TS:   items.join(",")
来源：http://ht.hnjuh.cn

Java: String.join(",", items)
来源：http://ew.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://xs.bjjhwx.cn

Ruby: items.join(",")
来源：http://nz.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://ch.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://kj.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://us.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://di.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://ha.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://of.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://te.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qd.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fa.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ko.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://vq.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://um.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oa.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://jl.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://gw.9csxet.cn

Java: String.format("%03d", 7)
来源：http://dk.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ye.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bd.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ef.nicolike.cn

[E11] 反转字符串
来源：http://br.wgjwhj.cn

Py:   s[::-1]
来源：http://ge.szxytkj.cn

PHP:  strrev($s);
来源：http://cl.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://zj.asd995.cn

TS:   [...s].reverse().join("")
来源：http://ou.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sl.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qb.shxzukj.cn

Ruby: s.reverse
来源：http://ya.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jw.nicolike.cn

[E12] 统计某字符出现次数
来源：http://th.yuntaijiaju.cn

Py:   s.count("a")
来源：http://ma.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://xk.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://hr.yuexingan06.cn

TS:   s.split("a").length - 1
来源：http://zw.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ic.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://vg.bookmarksfly.cn

Ruby: s.count("a")
来源：http://uv.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://ll.asd995.cn

[E13] 逐字符遍历
来源：http://zi.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://hu.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ek.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lq.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cw.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sg.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://do.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://az.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ig.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://nr.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lq.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lb.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yt.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nw.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pv.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://no.jctech888.com.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rj.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oo.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://no.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bg.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oe.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kx.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vj.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://aw.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xf.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fi.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sq.shxzukj.cn

[E16] 数字千分位
来源：http://wd.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://xy.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://bg.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uo.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vo.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cr.asd995.cn


<!-- 参考信息 -->