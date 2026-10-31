代发 wailian999

PHP:  sort($arr);
来源：http://ne.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kk.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ec.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pq.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vs.newstarts.cn

Ruby: arr.sort
来源：http://ar.yuntaijiaju.cn

C#:   list.Sort();
来源：http://qm.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mp.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kc.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uo.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://il.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mo.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kt.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yk.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nd.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gi.panjiajie.cn

[D11] 反转数组
来源：http://vo.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lq.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://jq.shtwfgs.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://my.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://ez.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://tv.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://ry.panjiajie.cn

Ruby: arr.reverse
来源：http://pu.lnxyls.cn

C#:   list.Reverse();
来源：http://kc.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://de.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://vc.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ll.nszjky.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://md.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lu.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ab.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://yj.lnxyls.cn

Ruby: arr.index(x)
来源：http://ik.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://ml.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://mc.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gv.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hq.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://jt.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://lt.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zx.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://on.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dh.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yw.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://gv.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qy.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ny.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://bf.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://om.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://av.panjiajie.cn

Go:   // 手写循环
来源：http://zx.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rq.shxzukj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rz.lnxyls.cn

[D15] 去重
来源：http://au.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cr.newstarts.cn

PHP:  array_unique($arr);
来源：http://rz.nszjky.cn

JS:   [...new Set(arr)]
来源：http://ss.gzmigu.cn

TS:   [...new Set(arr)]
来源：http://ub.huixiangedu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wd.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sc.nszjky.cn

Ruby: arr.uniq
来源：http://qa.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://kh.szxytkj.cn

[D16] 求和与平均值
来源：http://ys.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bu.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rt.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jg.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://al.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://id.wgjwhj.cn

Go:   // 手写循环累加
来源：http://ym.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qt.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://yj.huanxung.cn

[D17] 最大值与最小值
来源：http://ne.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://ul.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://hh.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kv.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://fv.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ba.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dy.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://tm.521024.cn

C#:   list.Max();  list.Min()
来源：http://gk.colortex.cn

[D18] 扁平化嵌套数组
来源：http://qu.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jg.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://ir.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ns.yuexingan06.cn

TS:   nested.flat();
来源：http://ek.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gw.wgjwhj.cn

Go:   // 手写双层循环
来源：http://zq.szsharing.cn

Ruby: nested.flatten
来源：http://un.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hk.colortex.cn

[D19] 按字段分组
来源：http://od.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jg.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nr.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mg.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://or.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tj.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://bo.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://oo.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zj.colortex.cn

[D20] 统计每个元素出现次数
来源：http://fr.szsharing.cn

Py:   Counter(arr)
来源：http://uz.nszjky.cn

PHP:  array_count_values($arr);
来源：http://pr.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tl.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pj.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gi.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://dw.shxzukj.cn

Ruby: arr.tally
来源：http://uk.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kb.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://mo.yuexingan06.cn

Py:   x in arr
来源：http://tu.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://hf.shxzukj.cn

JS:   arr.includes(x)
来源：http://cn.gzmigu.cn

TS:   arr.includes(x)
来源：http://qc.yuntaijiaju.cn

Java: list.contains(x)
来源：http://fc.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://xn.asd995.cn

Ruby: arr.include?(x)
来源：http://pl.muxihuayi.cn

C#:   list.Contains(x)
来源：http://tj.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://mc.huixinmuqiang.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tb.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://td.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://so.9csxet.cn

TS:   [...arr];
来源：http://cd.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://kt.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dd.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://ju.hahajie.cn

C#:   new List<int>(list);
来源：http://ng.szxytkj.cn

[D23] reduce 累积计算
来源：http://my.lnxyls.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://am.yuexingan06.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://du.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://or.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wk.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://aa.huixinmuqiang.cn

Go:   // 手写循环
来源：http://aq.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dx.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ag.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://ym.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ob.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hl.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bm.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ql.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vz.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ml.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qd.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sq.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://ee.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://th.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gt.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yg.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tt.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kg.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mc.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zq.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rn.muxihuayi.cn

[D26] 数组转字符串
来源：http://da.asd995.cn

Py:   ", ".join(map(str, arr))
来源：http://vq.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://gj.nszjky.cn

JS:   arr.join(", ")
来源：http://xf.521024.cn

TS:   arr.join(", ")
来源：http://al.colortex.cn

Java: String.join(", ", list)
来源：http://hp.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://zv.nszjky.cn

Ruby: arr.join(", ")
来源：http://pp.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://uu.gzmigu.cn

================================================================================
来源：http://mb.nicolike.cn

E. 字符串处理
来源：http://re.yuexingan06.cn

================================================================================
来源：http://qj.yuexingan06.cn

[E01] 拼接字符串
来源：http://sv.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ye.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tq.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tr.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iw.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ov.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hn.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nr.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qx.gzmigu.cn

[E02] 重复字符串
来源：http://il.jctech888.com.cn

Py:   "ab" * 3
来源：http://kj.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://gh.szsharing.cn

JS:   "ab".repeat(3)
来源：http://pq.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://qa.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://mh.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://nx.panjiajie.cn

Ruby: "ab" * 3
来源：http://hl.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uu.bookmarksfly.cn

[E03] 截取子串
来源：http://ty.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yc.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ni.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ed.colortex.cn

TS:   s.slice(1, 4)
来源：http://in.szsharing.cn

Java: s.substring(1, 4)
来源：http://ml.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ih.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kd.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://dj.szsharing.cn

[E04] 查找子串位置
来源：http://ph.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://iw.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://cl.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ll.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://qn.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://sm.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://br.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://um.asd995.cn

C#:   s.IndexOf("x")
来源：http://az.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rc.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gj.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ba.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sx.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://up.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vd.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lb.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wz.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cb.huixiangedu.cn

[E06] 替换子串
来源：http://pv.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ck.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://cl.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rm.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://qz.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sv.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ql.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://df.asd995.cn

C#:   s.Replace("a", "b")
来源：http://pv.szxytkj.cn

[E07] 按分隔符拆分
来源：http://ws.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://je.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://su.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hq.jianghongdianzi.cn

TS:   s.split(",")
来源：http://tf.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://aq.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wm.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://zv.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ov.9csxet.cn

[E08] 数组按分隔符合并
来源：http://oa.shxzukj.cn

Py:   ",".join(items)
来源：http://zt.lnxyls.cn

PHP:  implode(",", $items);
来源：http://ne.panjiajie.cn

JS:   items.join(",")
来源：http://lj.jctech888.com.cn

TS:   items.join(",")
来源：http://jn.wgjwhj.cn

Java: String.join(",", items)
来源：http://du.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://fs.nicolike.cn

Ruby: items.join(",")
来源：http://hu.szsharing.cn

C#:   string.Join(",", items)
来源：http://ov.hnjuh.cn

[E09] 去除所有空白字符
来源：http://bd.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hv.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bc.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://qp.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://by.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://kd.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xh.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gt.wgjwhj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ag.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://lv.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uf.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ec.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://he.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://gn.nszjky.cn

Java: String.format("%03d", 7)
来源：http://jj.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ob.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zb.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xv.szsharing.cn

[E11] 反转字符串
来源：http://te.nicolike.cn

Py:   s[::-1]
来源：http://vy.newstarts.cn

PHP:  strrev($s);
来源：http://jm.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://br.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://zx.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ij.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bx.shtwfgs.cn

Ruby: s.reverse
来源：http://uf.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lx.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://nu.521024.cn

Py:   s.count("a")
来源：http://ut.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://et.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://hh.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://qr.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nx.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://ea.lnxyls.cn

Ruby: s.count("a")
来源：http://mu.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://bg.nszjky.cn

[E13] 逐字符遍历
来源：http://az.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://re.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cs.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rt.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rk.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ql.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ic.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rn.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lo.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://yg.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lj.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zn.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vy.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jj.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vo.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qa.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ma.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cs.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://ky.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ra.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kg.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gl.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ee.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lh.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yx.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zz.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hw.lnxyls.cn

[E16] 数字千分位
来源：http://ps.9csxet.cn

Py:   f"{1234567:,}"
来源：http://vj.panjiajie.cn


<!-- 参考信息 -->