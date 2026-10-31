代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://lw.wgjwhj.cn

TS:   [...a, ...b];
来源：http://pa.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rr.wgjwhj.cn

Go:   append(a, b...)
来源：http://cx.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://kq.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://ma.newstarts.cn

[D09] 排序（升序）
来源：http://hd.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://py.hahajie.cn

PHP:  sort($arr);
来源：http://bi.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nb.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rh.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hf.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qk.jianghongdianzi.cn

Ruby: arr.sort
来源：http://lb.newstarts.cn

C#:   list.Sort();
来源：http://aq.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hx.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kx.szsharing.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sc.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mk.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vd.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dy.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://px.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pg.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ss.bookmarksfly.cn

[D11] 反转数组
来源：http://vf.hahajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fq.521024.cn

PHP:  array_reverse($arr);
来源：http://cn.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pi.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://df.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://ck.colortex.cn

Go:   slices.Reverse(arr)
来源：http://ea.hahajie.cn

Ruby: arr.reverse
来源：http://py.shxzukj.cn

C#:   list.Reverse();
来源：http://kf.newstarts.cn

[D12] 查找元素下标
来源：http://xm.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://it.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zw.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nh.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lt.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gj.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://av.hnjuh.cn

Ruby: arr.index(x)
来源：http://ml.9csxet.cn

C#:   list.IndexOf(x);
来源：http://wh.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://eh.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sb.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ts.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://ef.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://vq.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dq.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://up.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://iu.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://px.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://zs.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cq.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pm.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://nx.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://ed.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gj.panjiajie.cn

Go:   // 手写循环
来源：http://lb.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ha.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://eq.hnjuh.cn

[D15] 去重
来源：http://ir.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://us.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://fy.nszjky.cn

JS:   [...new Set(arr)]
来源：http://oo.asd995.cn

TS:   [...new Set(arr)]
来源：http://wt.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cl.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vl.chemitech.net.cn

Ruby: arr.uniq
来源：http://gf.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://sy.jctech888.com.cn

[D16] 求和与平均值
来源：http://to.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xa.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kc.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qj.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hb.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fg.lnxyls.cn

Go:   // 手写循环累加
来源：http://wu.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tl.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://ax.huanxung.cn

[D17] 最大值与最小值
来源：http://bh.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://am.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://fl.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gn.szsharing.cn

TS:   Math.max(...arr);
来源：http://py.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://po.521024.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ew.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://pu.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://ow.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://qt.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://so.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://ym.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ot.yuexingan06.cn

TS:   nested.flat();
来源：http://ij.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ak.gzmigu.cn

Go:   // 手写双层循环
来源：http://xi.huixinmuqiang.cn

Ruby: nested.flatten
来源：http://bp.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xd.chemitech.net.cn

[D19] 按字段分组
来源：http://tx.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uh.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ph.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yv.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qn.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fh.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://ih.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nf.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sl.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://pc.9csxet.cn

Py:   Counter(arr)
来源：http://zd.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://uq.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ka.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ix.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xy.huanxung.cn

Go:   // 手写 map[T]int
来源：http://sy.wgjwhj.cn

Ruby: arr.tally
来源：http://cr.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yd.nszjky.cn

[D21] 判断是否包含某元素
来源：http://qk.szxytkj.cn

Py:   x in arr
来源：http://su.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://bj.yuexingan06.cn

JS:   arr.includes(x)
来源：http://nj.asd995.cn

TS:   arr.includes(x)
来源：http://hu.jctech888.com.cn

Java: list.contains(x)
来源：http://hy.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://vt.nicolike.cn

Ruby: arr.include?(x)
来源：http://gn.jctech888.com.cn

C#:   list.Contains(x)
来源：http://tq.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://oj.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kh.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pv.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ix.panjiajie.cn

TS:   [...arr];
来源：http://ca.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://gn.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ph.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://ed.shxzukj.cn

C#:   new List<int>(list);
来源：http://vt.nicolike.cn

[D23] reduce 累积计算
来源：http://wt.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eh.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lu.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bk.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qd.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yr.chemitech.net.cn

Go:   // 手写循环
来源：http://uf.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ph.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mg.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://vl.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gw.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dh.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vr.colortex.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xh.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ho.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qs.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cm.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cn.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://eq.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yd.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zn.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ho.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yg.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pe.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://na.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gw.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ly.muxihuayi.cn

[D26] 数组转字符串
来源：http://ql.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://up.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://kl.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://kd.521024.cn

TS:   arr.join(", ")
来源：http://si.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://ym.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://ok.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://nm.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://uv.huixiangedu.cn

================================================================================
来源：http://ys.nszjky.cn

E. 字符串处理
来源：http://qe.nszjky.cn

================================================================================
来源：http://qu.wgjwhj.cn

[E01] 拼接字符串
来源：http://ob.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://am.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ec.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zw.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rp.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sj.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nc.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xf.haigaiapp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://de.asd995.cn

[E02] 重复字符串
来源：http://qk.bjjhwx.cn

Py:   "ab" * 3
来源：http://wj.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://aw.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://cz.nicolike.cn

TS:   "ab".repeat(3)
来源：http://vk.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://oe.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://pm.shxzskj.cn

Ruby: "ab" * 3
来源：http://zv.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sz.haigaiapp.cn

[E03] 截取子串
来源：http://gf.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nj.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hk.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yq.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://ke.panjiajie.cn

Java: s.substring(1, 4)
来源：http://jf.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nx.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ui.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://wi.hnjuh.cn

[E04] 查找子串位置
来源：http://hg.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://mt.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://bs.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vk.colortex.cn

TS:   s.indexOf("x")
来源：http://ga.521024.cn

Java: s.indexOf("x")
来源：http://pu.asd995.cn

Go:   strings.Index(s, "x")
来源：http://et.hahajie.cn

Ruby: s.index("x")
来源：http://ez.colortex.cn

C#:   s.IndexOf("x")
来源：http://va.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hc.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qo.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ta.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hw.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eq.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gk.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hj.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yj.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://en.szxytkj.cn

[E06] 替换子串
来源：http://ln.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mm.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://rk.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://by.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://am.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xt.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lk.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xe.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://aa.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://mh.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ph.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://py.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ld.wgjwhj.cn

TS:   s.split(",")
来源：http://dx.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xw.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://og.nszjky.cn

Ruby: s.split(",");  s.split
来源：http://rs.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qe.newstarts.cn

[E08] 数组按分隔符合并
来源：http://pd.muxihuayi.cn

Py:   ",".join(items)
来源：http://mo.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://vd.bookmarksfly.cn

JS:   items.join(",")
来源：http://ei.shxzskj.cn

TS:   items.join(",")
来源：http://pd.bjjhwx.cn

Java: String.join(",", items)
来源：http://nl.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://rb.panjiajie.cn

Ruby: items.join(",")
来源：http://qn.lnxyls.cn

C#:   string.Join(",", items)
来源：http://ea.panjiajie.cn

[E09] 去除所有空白字符
来源：http://hh.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://px.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cy.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://rx.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://vv.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://zt.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://du.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://al.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wd.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://yb.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zk.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ud.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://fx.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://si.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://ge.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://el.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ai.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yj.nicolike.cn

[E11] 反转字符串
来源：http://at.wgjwhj.cn

Py:   s[::-1]
来源：http://cn.shtwfgs.cn

PHP:  strrev($s);
来源：http://np.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://xh.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://kb.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kq.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rz.asd995.cn

Ruby: s.reverse
来源：http://rw.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://og.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://oa.haigaiapp.cn

Py:   s.count("a")
来源：http://zo.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://eh.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://dy.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://og.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://di.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://ex.shtwfgs.cn

Ruby: s.count("a")
来源：http://ta.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://cp.panjiajie.cn

[E13] 逐字符遍历
来源：http://cb.colortex.cn

Py:   for ch in s: print(ch)
来源：http://cv.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vt.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ht.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ym.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ls.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wd.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yx.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://co.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://ys.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ci.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zb.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wt.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mf.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yv.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://un.hnjuh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nc.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kw.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://zd.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pu.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://va.yuexingan06.cn


<!-- 参考信息 -->