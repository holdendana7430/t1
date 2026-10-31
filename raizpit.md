代发 wailian999

Java: list.size();
来源：http://pv.hnjuh.cn

Go:   len(arr)
来源：http://zf.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://es.haigaiapp.cn

C#:   list.Count;
来源：http://lm.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://ia.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xa.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://um.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://pf.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://di.szsharing.cn

Java: list.subList(1, 4);
来源：http://vs.panjiajie.cn

Go:   arr[1:4]
来源：http://bc.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://xy.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://zt.wgjwhj.cn

[D08] 合并两个数组
来源：http://xg.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://pz.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://ox.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fj.huixiangedu.cn

TS:   [...a, ...b];
来源：http://ht.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ru.jctech888.com.cn

Go:   append(a, b...)
来源：http://ct.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://fc.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://fe.nicolike.cn

[D09] 排序（升序）
来源：http://gh.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://kn.gzmigu.cn

PHP:  sort($arr);
来源：http://tg.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://do.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vj.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ug.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eh.jianghongdianzi.cn

Ruby: arr.sort
来源：http://sz.wgjwhj.cn

C#:   list.Sort();
来源：http://fs.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jw.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jn.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rr.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gf.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jy.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eu.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xs.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ee.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kb.9csxet.cn

[D11] 反转数组
来源：http://ay.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ti.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://ol.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qj.hahajie.cn

TS:   [...arr].reverse();
来源：http://tq.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://om.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://yq.bookmarksfly.cn

Ruby: arr.reverse
来源：http://fe.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://my.hahajie.cn

[D12] 查找元素下标
来源：http://iy.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://jt.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://to.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mo.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zz.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wr.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://kc.huanxung.cn

Ruby: arr.index(x)
来源：http://ve.9csxet.cn

C#:   list.IndexOf(x);
来源：http://lk.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://ko.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fe.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mk.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://sa.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://ts.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jd.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sj.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://db.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wy.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://od.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ig.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nu.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://tl.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://xz.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://th.szsharing.cn

Go:   // 手写循环
来源：http://qe.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bf.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mx.chemitech.net.cn

[D15] 去重
来源：http://et.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zy.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://ff.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://en.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://gf.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://go.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xa.panjiajie.cn

Ruby: arr.uniq
来源：http://qj.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://rj.muxihuayi.cn

[D16] 求和与平均值
来源：http://bk.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yu.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://py.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xu.chemitech.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kp.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wr.huanxung.cn

Go:   // 手写循环累加
来源：http://lu.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gr.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://um.chemitech.net.cn

[D17] 最大值与最小值
来源：http://zb.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://vp.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://ly.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ce.newstarts.cn

TS:   Math.max(...arr);
来源：http://hg.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kn.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://he.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://wy.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://yp.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://xb.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rd.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://ls.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ds.yuexingan06.cn

TS:   nested.flat();
来源：http://zl.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yg.colortex.cn

Go:   // 手写双层循环
来源：http://fd.chemitech.net.cn

Ruby: nested.flatten
来源：http://ow.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yb.nicolike.cn

[D19] 按字段分组
来源：http://dm.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lo.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bl.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cy.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ho.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qj.521024.cn

Go:   // 手写 map[string][]T
来源：http://tp.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fu.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fp.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://sb.asd995.cn

Py:   Counter(arr)
来源：http://ji.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://ng.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ti.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pr.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fw.521024.cn

Go:   // 手写 map[T]int
来源：http://xp.chemitech.net.cn

Ruby: arr.tally
来源：http://cj.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fj.9csxet.cn

[D21] 判断是否包含某元素
来源：http://ae.shxzskj.cn

Py:   x in arr
来源：http://wq.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://de.asd995.cn

JS:   arr.includes(x)
来源：http://xi.szxytkj.cn

TS:   arr.includes(x)
来源：http://ei.jctech888.com.cn

Java: list.contains(x)
来源：http://hh.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://ag.shxzukj.cn

Ruby: arr.include?(x)
来源：http://yt.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://gz.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://ev.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vk.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ql.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ps.szsharing.cn

TS:   [...arr];
来源：http://bd.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://nn.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ve.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://fz.lnxyls.cn

C#:   new List<int>(list);
来源：http://ti.szsharing.cn

[D23] reduce 累积计算
来源：http://tu.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vn.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hh.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://na.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uh.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ew.wgjwhj.cn

Go:   // 手写循环
来源：http://yt.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uf.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vw.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://cp.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kb.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ij.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hf.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dk.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ht.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uq.hnjuh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hf.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uu.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://ox.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hd.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qt.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ao.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://br.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ql.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yp.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hb.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zv.lnxyls.cn

[D26] 数组转字符串
来源：http://mn.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://vx.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://qp.gzmigu.cn

JS:   arr.join(", ")
来源：http://pu.bjjhwx.cn

TS:   arr.join(", ")
来源：http://om.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://pq.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://xs.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://bc.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://po.hahajie.cn

================================================================================
来源：http://dh.jctech888.com.cn

E. 字符串处理
来源：http://zc.jctech888.com.cn

================================================================================
来源：http://aq.jctech888.com.cn

[E01] 拼接字符串
来源：http://sf.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bu.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ht.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rv.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rw.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ue.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tm.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vs.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hk.asd995.cn

[E02] 重复字符串
来源：http://ar.hnjuh.cn

Py:   "ab" * 3
来源：http://ck.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://na.szsharing.cn

JS:   "ab".repeat(3)
来源：http://wb.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://dp.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://iq.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://sl.jctech888.com.cn

Ruby: "ab" * 3
来源：http://ur.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qd.yuntaijiaju.cn

[E03] 截取子串
来源：http://ad.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eo.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ba.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hw.hahajie.cn

TS:   s.slice(1, 4)
来源：http://xp.panjiajie.cn

Java: s.substring(1, 4)
来源：http://dg.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jq.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zb.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://ox.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://hm.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://st.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://qy.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yd.panjiajie.cn

TS:   s.indexOf("x")
来源：http://xz.lnxyls.cn

Java: s.indexOf("x")
来源：http://il.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://qr.wgjwhj.cn

Ruby: s.index("x")
来源：http://ue.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://ob.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ov.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://je.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uz.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qv.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wq.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mn.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eg.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yo.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bm.huanxung.cn

[E06] 替换子串
来源：http://cn.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xn.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://bl.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bj.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://pk.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fb.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hc.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rt.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://fe.nszjky.cn

[E07] 按分隔符拆分
来源：http://kp.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://an.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://di.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jx.chemitech.net.cn

TS:   s.split(",")
来源：http://bw.gzmigu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sx.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ak.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://lu.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mg.szsharing.cn

[E08] 数组按分隔符合并
来源：http://sz.jctech888.com.cn

Py:   ",".join(items)
来源：http://vn.521024.cn

PHP:  implode(",", $items);
来源：http://od.shxzukj.cn

JS:   items.join(",")
来源：http://sp.haigaiapp.cn

TS:   items.join(",")
来源：http://hv.lnxyls.cn

Java: String.join(",", items)
来源：http://dg.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://ll.szxytkj.cn

Ruby: items.join(",")
来源：http://ot.huanxung.cn

C#:   string.Join(",", items)
来源：http://zj.hahajie.cn

[E09] 去除所有空白字符
来源：http://ki.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rb.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hg.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://da.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://ue.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://fu.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://km.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jp.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mu.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://no.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sr.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tc.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://pz.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://yy.huanxung.cn

Java: String.format("%03d", 7)
来源：http://ls.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wi.shxzskj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uv.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ur.szsharing.cn

[E11] 反转字符串
来源：http://lw.jctech888.com.cn

Py:   s[::-1]
来源：http://oj.hnjuh.cn

PHP:  strrev($s);
来源：http://tb.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://yt.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://ti.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xu.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uo.shxzskj.cn

Ruby: s.reverse
来源：http://zu.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sr.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://jq.haigaiapp.cn

Py:   s.count("a")
来源：http://lo.wgjwhj.cn

PHP:  substr_count($s, "a");
来源：http://ep.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://ar.colortex.cn

TS:   s.split("a").length - 1
来源：http://vf.colortex.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ow.9csxet.cn

Go:   strings.Count(s, "a")
来源：http://vg.asd995.cn

Ruby: s.count("a")
来源：http://ze.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://hk.shxzskj.cn

[E13] 逐字符遍历
来源：http://da.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://wo.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gs.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mz.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://th.jianghongdianzi.cn


<!-- 参考信息 -->