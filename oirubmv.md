代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://fy.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://dq.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://nh.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://dw.jctech888.com.cn

PHP:  sort($arr);
来源：http://ea.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vm.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fg.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lf.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qk.panjiajie.cn

Ruby: arr.sort
来源：http://hd.colortex.cn

C#:   list.Sort();
来源：http://tm.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cy.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://av.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ok.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bx.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wh.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lj.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zv.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yh.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yk.lnxyls.cn

[D11] 反转数组
来源：http://dh.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gf.521024.cn

PHP:  array_reverse($arr);
来源：http://nr.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kn.huixinmuqiang.cn

TS:   [...arr].reverse();
来源：http://eh.hahajie.cn

Java: Collections.reverse(list);
来源：http://km.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://rg.shxzskj.cn

Ruby: arr.reverse
来源：http://zf.shtwfgs.cn

C#:   list.Reverse();
来源：http://zg.haigaiapp.cn

[D12] 查找元素下标
来源：http://jt.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://da.newstarts.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zw.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://el.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cv.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aw.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://so.newstarts.cn

Ruby: arr.index(x)
来源：http://tj.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://mf.muxihuayi.cn

[D13] 过滤（保留满足条件的）
来源：http://zd.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gg.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kq.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://td.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://ya.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://an.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fn.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dr.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jz.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://ds.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eg.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ml.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://ib.huixiangedu.cn

TS:   arr.map(x => x * 2)
来源：http://ck.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zi.asd995.cn

Go:   // 手写循环
来源：http://it.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tk.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zo.hahajie.cn

[D15] 去重
来源：http://yh.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ou.asd995.cn

PHP:  array_unique($arr);
来源：http://tt.9csxet.cn

JS:   [...new Set(arr)]
来源：http://qn.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://gx.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fi.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://du.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://an.521024.cn

C#:   list.Distinct().ToList()
来源：http://ku.hnjuh.cn

[D16] 求和与平均值
来源：http://ym.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nj.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ja.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jz.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jm.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kf.shxzskj.cn

Go:   // 手写循环累加
来源：http://io.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kw.huixinmuqiang.cn

C#:   list.Sum();  list.Average()
来源：http://bb.szsharing.cn

[D17] 最大值与最小值
来源：http://qe.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://og.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://vf.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://aq.shxzskj.cn

TS:   Math.max(...arr);
来源：http://qt.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uc.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rb.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://ml.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://lc.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://iy.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ad.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://xr.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gx.shtwfgs.cn

TS:   nested.flat();
来源：http://db.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qg.wgjwhj.cn

Go:   // 手写双层循环
来源：http://db.jianghongdianzi.cn

Ruby: nested.flatten
来源：http://ab.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hs.9csxet.cn

[D19] 按字段分组
来源：http://nk.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ab.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hb.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yg.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vw.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jq.jianghongdianzi.cn

Go:   // 手写 map[string][]T
来源：http://yc.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://as.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cr.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://ni.muxihuayi.cn

Py:   Counter(arr)
来源：http://wk.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://zk.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yy.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tx.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://at.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://ra.shtwfgs.cn

Ruby: arr.tally
来源：http://nl.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jy.colortex.cn

[D21] 判断是否包含某元素
来源：http://ju.newstarts.cn

Py:   x in arr
来源：http://du.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://do.chemitech.net.cn

JS:   arr.includes(x)
来源：http://ea.haigaiapp.cn

TS:   arr.includes(x)
来源：http://qs.jianghongdianzi.cn

Java: list.contains(x)
来源：http://vs.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://ak.shxzskj.cn

Ruby: arr.include?(x)
来源：http://vv.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://ah.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://uo.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ow.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kt.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vg.newstarts.cn

TS:   [...arr];
来源：http://ho.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://ee.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rp.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://sx.lnxyls.cn

C#:   new List<int>(list);
来源：http://gv.9csxet.cn

[D23] reduce 累积计算
来源：http://tq.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ba.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yq.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pp.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://st.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wg.huixinmuqiang.cn

Go:   // 手写循环
来源：http://ap.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xh.hahajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fu.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://lu.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qj.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oh.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zq.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mw.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gw.szxytkj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uk.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lf.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iy.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://cx.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sw.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mh.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vo.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lt.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dk.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ku.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gy.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ke.colortex.cn

[D26] 数组转字符串
来源：http://dd.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://qb.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://mr.szxytkj.cn

JS:   arr.join(", ")
来源：http://nb.nszjky.cn

TS:   arr.join(", ")
来源：http://fh.hahajie.cn

Java: String.join(", ", list)
来源：http://zk.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://gj.hnjuh.cn

Ruby: arr.join(", ")
来源：http://hn.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://xi.nszjky.cn

================================================================================
来源：http://fa.bookmarksfly.cn

E. 字符串处理
来源：http://wa.huixiangedu.cn

================================================================================
来源：http://jo.bookmarksfly.cn

[E01] 拼接字符串
来源：http://za.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cn.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bv.hnjuh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nc.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lh.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://im.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cr.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hm.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xv.yuexingan06.cn

[E02] 重复字符串
来源：http://sd.hahajie.cn

Py:   "ab" * 3
来源：http://gw.gzmigu.cn

PHP:  str_repeat("ab", 3);
来源：http://cq.asd995.cn

JS:   "ab".repeat(3)
来源：http://kb.nszjky.cn

TS:   "ab".repeat(3)
来源：http://df.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://iv.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://vb.wgjwhj.cn

Ruby: "ab" * 3
来源：http://ao.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qp.panjiajie.cn

[E03] 截取子串
来源：http://rd.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://va.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qf.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ob.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://gy.shxzskj.cn

Java: s.substring(1, 4)
来源：http://pt.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eu.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lq.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://ym.bookmarksfly.cn

[E04] 查找子串位置
来源：http://ln.szsharing.cn

Py:   s.find("x");  s.index("x")
来源：http://oc.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://io.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://td.newstarts.cn

TS:   s.indexOf("x")
来源：http://ld.nszjky.cn

Java: s.indexOf("x")
来源：http://al.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://sw.521024.cn

Ruby: s.index("x")
来源：http://no.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://nd.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ey.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yt.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ao.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rz.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sv.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qp.huanxung.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://um.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uq.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iq.haigaiapp.cn

[E06] 替换子串
来源：http://kz.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oe.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://na.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cn.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://ay.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wh.colortex.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fq.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eu.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://iv.hahajie.cn

[E07] 按分隔符拆分
来源：http://ns.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sr.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oi.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nm.chemitech.net.cn

TS:   s.split(",")
来源：http://yk.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://in.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oi.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://su.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jp.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://we.colortex.cn

Py:   ",".join(items)
来源：http://rp.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://gs.szxytkj.cn

JS:   items.join(",")
来源：http://vn.nicolike.cn

TS:   items.join(",")
来源：http://bk.yuexingan06.cn

Java: String.join(",", items)
来源：http://wl.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://ci.newstarts.cn

Ruby: items.join(",")
来源：http://xh.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://ax.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://sn.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ub.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://np.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://hw.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://nh.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://wf.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://df.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hb.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://es.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://wr.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nx.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://po.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://oz.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://ff.asd995.cn

Java: String.format("%03d", 7)
来源：http://lg.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rp.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hf.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pm.jctech888.com.cn

[E11] 反转字符串
来源：http://yf.nszjky.cn

Py:   s[::-1]
来源：http://is.szsharing.cn

PHP:  strrev($s);
来源：http://dx.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://tz.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://xm.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ap.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sl.bookmarksfly.cn

Ruby: s.reverse
来源：http://mi.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dv.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://pn.bookmarksfly.cn

Py:   s.count("a")
来源：http://el.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://ph.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://nx.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://jk.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yh.colortex.cn

Go:   strings.Count(s, "a")
来源：http://bm.asd995.cn

Ruby: s.count("a")
来源：http://wn.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://gf.haigaiapp.cn

[E13] 逐字符遍历
来源：http://uz.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://su.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bg.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dv.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gl.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sj.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hu.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yj.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://il.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://zt.huixiangedu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cj.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jz.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jm.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lr.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://te.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gs.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wf.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bc.huixinmuqiang.cn

[E15] HTML 转义 / 反转义
来源：http://tj.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://st.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vx.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pa.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://oh.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mf.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://di.newstarts.cn


<!-- 参考信息 -->