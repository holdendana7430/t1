代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://eu.huixiangedu.cn

[D08] 合并两个数组
来源：http://sv.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://pv.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://yv.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ts.shxzukj.cn

TS:   [...a, ...b];
来源：http://gf.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nx.shtwfgs.cn

Go:   append(a, b...)
来源：http://kz.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://vq.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://pn.asd995.cn

[D09] 排序（升序）
来源：http://qz.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://ll.bjjhwx.cn

PHP:  sort($arr);
来源：http://do.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://id.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ru.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://aq.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xw.newstarts.cn

Ruby: arr.sort
来源：http://nw.gzmigu.cn

C#:   list.Sort();
来源：http://yp.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ry.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uw.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ft.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ve.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oo.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pr.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tg.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gj.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rj.bookmarksfly.cn

[D11] 反转数组
来源：http://fp.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yz.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://iw.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jt.shxzukj.cn

TS:   [...arr].reverse();
来源：http://wj.colortex.cn

Java: Collections.reverse(list);
来源：http://ib.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://nw.panjiajie.cn

Ruby: arr.reverse
来源：http://dg.asd995.cn

C#:   list.Reverse();
来源：http://yw.nszjky.cn

[D12] 查找元素下标
来源：http://df.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://qa.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cv.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wb.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cv.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dh.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://bx.nicolike.cn

Ruby: arr.index(x)
来源：http://oc.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://ma.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://dq.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ue.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zk.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://xb.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://ui.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hh.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mv.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yz.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pe.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://bf.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ze.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://he.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://vo.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://yf.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ew.muxihuayi.cn

Go:   // 手写循环
来源：http://sb.bjjhwx.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wn.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fb.chemitech.net.cn

[D15] 去重
来源：http://zg.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zm.nszjky.cn

PHP:  array_unique($arr);
来源：http://jq.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://pu.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://kh.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qn.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dx.9csxet.cn

Ruby: arr.uniq
来源：http://sl.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://ex.nszjky.cn

[D16] 求和与平均值
来源：http://mt.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tt.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vk.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tq.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fw.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pa.lnxyls.cn

Go:   // 手写循环累加
来源：http://nx.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xz.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://mc.wgjwhj.cn

[D17] 最大值与最小值
来源：http://ne.asd995.cn

Py:   max(arr);  min(arr)
来源：http://ne.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://rj.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yy.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://wn.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://be.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yq.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://pt.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://wm.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://ih.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://no.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://lv.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cd.asd995.cn

TS:   nested.flat();
来源：http://nk.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rq.yuexingan06.cn

Go:   // 手写双层循环
来源：http://cs.lnxyls.cn

Ruby: nested.flatten
来源：http://ob.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nj.shtwfgs.cn

[D19] 按字段分组
来源：http://fo.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xw.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eh.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zk.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qe.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gh.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://vc.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ra.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yv.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://oh.shxzskj.cn

Py:   Counter(arr)
来源：http://qk.nszjky.cn

PHP:  array_count_values($arr);
来源：http://pi.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wg.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vv.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sy.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://ls.gzmigu.cn

Ruby: arr.tally
来源：http://eo.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zg.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://yr.wgjwhj.cn

Py:   x in arr
来源：http://jl.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://vg.shxzskj.cn

JS:   arr.includes(x)
来源：http://nj.szxytkj.cn

TS:   arr.includes(x)
来源：http://yf.huixinmuqiang.cn

Java: list.contains(x)
来源：http://hm.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://di.nszjky.cn

Ruby: arr.include?(x)
来源：http://lo.huixiangedu.cn

C#:   list.Contains(x)
来源：http://tc.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://ax.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gq.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ma.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nh.newstarts.cn

TS:   [...arr];
来源：http://jl.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://ud.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kv.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://bt.colortex.cn

C#:   new List<int>(list);
来源：http://ar.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://hc.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gy.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mc.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qt.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ah.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ea.shxzskj.cn

Go:   // 手写循环
来源：http://rn.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pk.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sz.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://sq.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ra.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rv.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sp.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ie.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xr.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yo.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tu.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ow.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://lz.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rv.521024.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eg.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bu.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lw.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ll.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://je.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qe.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vx.huixinmuqiang.cn

[D26] 数组转字符串
来源：http://dn.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://ym.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://ph.lnxyls.cn

JS:   arr.join(", ")
来源：http://gq.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://jk.hnjuh.cn

Java: String.join(", ", list)
来源：http://bz.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://dn.asd995.cn

Ruby: arr.join(", ")
来源：http://ce.colortex.cn

C#:   string.Join(", ", list)
来源：http://bw.nicolike.cn

================================================================================
来源：http://ks.panjiajie.cn

E. 字符串处理
来源：http://iz.shxzukj.cn

================================================================================
来源：http://fu.wgjwhj.cn

[E01] 拼接字符串
来源：http://ju.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lz.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bo.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yb.jianghongdianzi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iq.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sy.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sl.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tt.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ly.newstarts.cn

[E02] 重复字符串
来源：http://hk.jctech888.com.cn

Py:   "ab" * 3
来源：http://dl.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://af.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://cf.hahajie.cn

TS:   "ab".repeat(3)
来源：http://pn.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://uw.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://jl.szxytkj.cn

Ruby: "ab" * 3
来源：http://yw.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wr.wgjwhj.cn

[E03] 截取子串
来源：http://bh.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kd.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gd.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kh.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://as.szsharing.cn

Java: s.substring(1, 4)
来源：http://gn.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zz.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ta.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://oe.colortex.cn

[E04] 查找子串位置
来源：http://zz.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://no.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://ll.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jc.huanxung.cn

TS:   s.indexOf("x")
来源：http://tl.newstarts.cn

Java: s.indexOf("x")
来源：http://aj.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://lq.szsharing.cn

Ruby: s.index("x")
来源：http://fk.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://ap.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qk.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://my.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aw.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://px.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uf.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ae.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ya.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iy.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qg.yuexingan06.cn

[E06] 替换子串
来源：http://rb.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://km.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://ul.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eq.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://fk.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ez.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yz.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ls.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://ws.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://gw.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rj.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lt.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://em.nszjky.cn

TS:   s.split(",")
来源：http://ou.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://op.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vy.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://kp.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ex.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://ao.bookmarksfly.cn

Py:   ",".join(items)
来源：http://bi.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://ko.huanxung.cn

JS:   items.join(",")
来源：http://ep.colortex.cn

TS:   items.join(",")
来源：http://dz.newstarts.cn

Java: String.join(",", items)
来源：http://yu.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://vt.gzmigu.cn

Ruby: items.join(",")
来源：http://lx.nszjky.cn

C#:   string.Join(",", items)
来源：http://rd.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://es.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hh.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rx.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://hk.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://vl.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://zq.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uf.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dy.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tt.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://jp.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dz.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ly.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://yk.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://pp.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://dd.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://db.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ny.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sb.huixinmuqiang.cn

[E11] 反转字符串
来源：http://au.huanxung.cn

Py:   s[::-1]
来源：http://gg.huanxung.cn

PHP:  strrev($s);
来源：http://on.asd995.cn

JS:   [...s].reverse().join("")
来源：http://bh.jctech888.com.cn

TS:   [...s].reverse().join("")
来源：http://fl.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://aa.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ji.newstarts.cn

Ruby: s.reverse
来源：http://od.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ht.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://sd.hahajie.cn

Py:   s.count("a")
来源：http://bp.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://ah.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://jt.nicolike.cn

TS:   s.split("a").length - 1
来源：http://fu.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bq.huixinmuqiang.cn

Go:   strings.Count(s, "a")
来源：http://hb.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://yt.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://jr.haigaiapp.cn

[E13] 逐字符遍历
来源：http://kb.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://pd.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qj.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rm.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zg.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bo.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uf.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qm.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cm.shtwfgs.cn

[E14] URL 编码与 Base64
来源：http://ut.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fl.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://za.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mc.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wc.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qb.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rb.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hw.9csxet.cn


<!-- 参考信息 -->