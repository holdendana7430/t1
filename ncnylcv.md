代发 wailian999

PHP:  sort($arr);
来源：http://tb.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hq.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ft.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://eq.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iv.muxihuayi.cn

Ruby: arr.sort
来源：http://ge.9csxet.cn

C#:   list.Sort();
来源：http://sj.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nz.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kh.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://he.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vn.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zt.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dt.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gd.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://am.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lv.bjjhwx.cn

[D11] 反转数组
来源：http://tp.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wz.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://st.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ef.shxzskj.cn

TS:   [...arr].reverse();
来源：http://fp.gzmigu.cn

Java: Collections.reverse(list);
来源：http://pa.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://xq.521024.cn

Ruby: arr.reverse
来源：http://up.huanxung.cn

C#:   list.Reverse();
来源：http://ck.hnjuh.cn

[D12] 查找元素下标
来源：http://mp.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://ga.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tl.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kx.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ei.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ub.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://yd.haigaiapp.cn

Ruby: arr.index(x)
来源：http://ls.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://zx.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://ch.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qi.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hr.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://cn.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://fh.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hy.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wc.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pv.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tb.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://ln.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mw.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vu.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://yj.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://qp.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ou.nicolike.cn

Go:   // 手写循环
来源：http://di.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lb.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cm.colortex.cn

[D15] 去重
来源：http://sh.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ai.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://tz.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://dn.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://xq.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nk.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://oj.newstarts.cn

Ruby: arr.uniq
来源：http://cp.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://af.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://sz.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xc.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jn.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dt.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lz.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lt.newstarts.cn

Go:   // 手写循环累加
来源：http://ai.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ij.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://wa.wgjwhj.cn

[D17] 最大值与最小值
来源：http://wr.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://sg.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://kr.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xn.szsharing.cn

TS:   Math.max(...arr);
来源：http://hv.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fd.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mm.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://vh.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://jd.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://eq.521024.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://th.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://sb.shxzskj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ye.shtwfgs.cn

TS:   nested.flat();
来源：http://qc.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qz.lnxyls.cn

Go:   // 手写双层循环
来源：http://uc.huanxung.cn

Ruby: nested.flatten
来源：http://zp.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lf.chemitech.net.cn

[D19] 按字段分组
来源：http://af.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zr.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ge.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bx.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rw.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zk.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://ed.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dj.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://na.521024.cn

[D20] 统计每个元素出现次数
来源：http://ip.9csxet.cn

Py:   Counter(arr)
来源：http://kz.huanxung.cn

PHP:  array_count_values($arr);
来源：http://ao.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ps.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ae.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pl.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://li.yuexingan06.cn

Ruby: arr.tally
来源：http://ga.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://at.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://zt.shxzskj.cn

Py:   x in arr
来源：http://ae.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://ap.shtwfgs.cn

JS:   arr.includes(x)
来源：http://je.huanxung.cn

TS:   arr.includes(x)
来源：http://vi.yuntaijiaju.cn

Java: list.contains(x)
来源：http://el.521024.cn

Go:   slices.Contains(arr, x)
来源：http://hv.hahajie.cn

Ruby: arr.include?(x)
来源：http://yt.huanxung.cn

C#:   list.Contains(x)
来源：http://jr.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://kc.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://at.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rd.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ac.szsharing.cn

TS:   [...arr];
来源：http://sf.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://aj.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jd.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://ji.nszjky.cn

C#:   new List<int>(list);
来源：http://vl.shtwfgs.cn

[D23] reduce 累积计算
来源：http://qg.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hb.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://la.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ia.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ss.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nn.shxzskj.cn

Go:   // 手写循环
来源：http://st.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://we.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oh.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://yt.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ih.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://me.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xm.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yx.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ze.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ey.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ag.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ci.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://ta.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bv.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ij.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pm.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bp.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cz.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yx.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ah.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zw.huanxung.cn

[D26] 数组转字符串
来源：http://hy.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://hw.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://zw.gzmigu.cn

JS:   arr.join(", ")
来源：http://ed.chemitech.net.cn

TS:   arr.join(", ")
来源：http://wg.chemitech.net.cn

Java: String.join(", ", list)
来源：http://dx.hahajie.cn

Go:   strings.Join(strs, ", ")
来源：http://zr.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://xm.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://zm.szxytkj.cn

================================================================================
来源：http://yl.9csxet.cn

E. 字符串处理
来源：http://ls.lnxyls.cn

================================================================================
来源：http://ez.shtwfgs.cn

[E01] 拼接字符串
来源：http://dy.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yy.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uy.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lq.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://er.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wn.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yy.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qu.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nd.bookmarksfly.cn

[E02] 重复字符串
来源：http://hh.bookmarksfly.cn

Py:   "ab" * 3
来源：http://mf.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://wp.9csxet.cn

JS:   "ab".repeat(3)
来源：http://po.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://tw.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://bl.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://jd.asd995.cn

Ruby: "ab" * 3
来源：http://lu.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qc.huixiangedu.cn

[E03] 截取子串
来源：http://je.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ix.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lw.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://of.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://kn.szxytkj.cn

Java: s.substring(1, 4)
来源：http://vj.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ih.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ra.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://bc.hnjuh.cn

[E04] 查找子串位置
来源：http://mj.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://bc.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://kg.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lj.szxytkj.cn

TS:   s.indexOf("x")
来源：http://xd.521024.cn

Java: s.indexOf("x")
来源：http://qq.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://sx.shtwfgs.cn

Ruby: s.index("x")
来源：http://uj.9csxet.cn

C#:   s.IndexOf("x")
来源：http://xx.huanxung.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tz.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ez.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ih.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dy.shxzskj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qh.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rg.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bb.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gv.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ag.521024.cn

[E06] 替换子串
来源：http://nb.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iv.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://pa.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gj.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://ou.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bx.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wa.asd995.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ni.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://nh.nicolike.cn

[E07] 按分隔符拆分
来源：http://fp.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kj.muxihuayi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://py.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zu.bjjhwx.cn

TS:   s.split(",")
来源：http://wd.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wr.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://al.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://rf.muxihuayi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sl.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://fi.yuexingan06.cn

Py:   ",".join(items)
来源：http://rh.shxzskj.cn

PHP:  implode(",", $items);
来源：http://uy.yuntaijiaju.cn

JS:   items.join(",")
来源：http://lu.huanxung.cn

TS:   items.join(",")
来源：http://rc.hnjuh.cn

Java: String.join(",", items)
来源：http://tv.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://rs.521024.cn

Ruby: items.join(",")
来源：http://mw.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://sa.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://ip.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ck.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pg.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://vn.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://gh.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://dk.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yn.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yo.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ay.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://pb.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://na.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qy.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://nw.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://mo.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://ll.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yp.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://il.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ce.asd995.cn

[E11] 反转字符串
来源：http://jb.huixiangedu.cn

Py:   s[::-1]
来源：http://np.panjiajie.cn

PHP:  strrev($s);
来源：http://du.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://ix.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://xa.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vc.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vv.nszjky.cn

Ruby: s.reverse
来源：http://nx.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qi.521024.cn

[E12] 统计某字符出现次数
来源：http://qw.9csxet.cn

Py:   s.count("a")
来源：http://ep.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://fo.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://rx.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://ih.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://my.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://hf.gzmigu.cn

Ruby: s.count("a")
来源：http://ag.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://aj.nicolike.cn

[E13] 逐字符遍历
来源：http://up.colortex.cn

Py:   for ch in s: print(ch)
来源：http://ae.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rx.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dd.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dk.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gg.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hr.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wp.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dh.nicolike.cn

[E14] URL 编码与 Base64
来源：http://lc.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://of.gzmigu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ob.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yz.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://om.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bm.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://id.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wn.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fw.huixinmuqiang.cn

[E15] HTML 转义 / 反转义
来源：http://gn.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://in.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kd.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://je.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pe.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iz.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nj.huixinmuqiang.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cf.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ql.yuntaijiaju.cn

[E16] 数字千分位
来源：http://pq.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://xu.shxzskj.cn


<!-- 参考信息 -->