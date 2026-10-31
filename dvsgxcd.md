代发 wailian999

Java: list.size();
来源：http://bj.panjiajie.cn

Go:   len(arr)
来源：http://cq.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://ey.haigaiapp.cn

C#:   list.Count;
来源：http://bh.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://qg.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rx.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pn.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://xy.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://ry.9csxet.cn

Java: list.subList(1, 4);
来源：http://pr.asd995.cn

Go:   arr[1:4]
来源：http://nb.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://ne.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://ja.chemitech.net.cn

[D08] 合并两个数组
来源：http://tl.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://ul.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://ne.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pd.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://gv.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ic.szsharing.cn

Go:   append(a, b...)
来源：http://ht.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://bd.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://sa.shxzskj.cn

[D09] 排序（升序）
来源：http://lb.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://tm.521024.cn

PHP:  sort($arr);
来源：http://wh.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gu.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://eq.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bm.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fg.huixinmuqiang.cn

Ruby: arr.sort
来源：http://kd.muxihuayi.cn

C#:   list.Sort();
来源：http://uh.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bh.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fm.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yg.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zo.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dc.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wb.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://un.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ss.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rx.gzmigu.cn

[D11] 反转数组
来源：http://co.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ch.9csxet.cn

PHP:  array_reverse($arr);
来源：http://ey.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hf.nszjky.cn

TS:   [...arr].reverse();
来源：http://aj.szsharing.cn

Java: Collections.reverse(list);
来源：http://az.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://dq.szsharing.cn

Ruby: arr.reverse
来源：http://qx.chemitech.net.cn

C#:   list.Reverse();
来源：http://dr.nszjky.cn

[D12] 查找元素下标
来源：http://si.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://ev.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lq.huanxung.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bu.shtwfgs.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kh.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ua.521024.cn

Go:   slices.Index(arr, x)
来源：http://jv.521024.cn

Ruby: arr.index(x)
来源：http://cl.nszjky.cn

C#:   list.IndexOf(x);
来源：http://pv.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://eg.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ah.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bf.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://na.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://fe.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iq.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qt.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://it.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sx.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://iw.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lk.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ce.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://dw.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://my.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vp.muxihuayi.cn

Go:   // 手写循环
来源：http://io.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mx.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://it.jctech888.com.cn

[D15] 去重
来源：http://wt.bjjhwx.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nw.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://xp.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://lr.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://do.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bc.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ho.wgjwhj.cn

Ruby: arr.uniq
来源：http://ru.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://xz.muxihuayi.cn

[D16] 求和与平均值
来源：http://pj.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hq.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lx.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ry.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ld.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://to.szsharing.cn

Go:   // 手写循环累加
来源：http://cm.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sn.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://sn.bjjhwx.cn

[D17] 最大值与最小值
来源：http://it.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://ou.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://fb.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hb.shxzskj.cn

TS:   Math.max(...arr);
来源：http://ch.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ig.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vj.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://xa.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://fi.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://pf.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pm.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://zo.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nh.bjjhwx.cn

TS:   nested.flat();
来源：http://oq.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sh.nszjky.cn

Go:   // 手写双层循环
来源：http://ki.haigaiapp.cn

Ruby: nested.flatten
来源：http://rc.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bb.huixiangedu.cn

[D19] 按字段分组
来源：http://sv.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tk.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sn.colortex.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://em.gzmigu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hc.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rx.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://yb.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://th.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wr.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://ru.colortex.cn

Py:   Counter(arr)
来源：http://ft.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://xf.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://io.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rc.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sb.colortex.cn

Go:   // 手写 map[T]int
来源：http://mf.colortex.cn

Ruby: arr.tally
来源：http://wh.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zt.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://tc.wgjwhj.cn

Py:   x in arr
来源：http://pw.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://re.chemitech.net.cn

JS:   arr.includes(x)
来源：http://ti.panjiajie.cn

TS:   arr.includes(x)
来源：http://db.wgjwhj.cn

Java: list.contains(x)
来源：http://vn.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://jr.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://kw.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://mb.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://vo.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dh.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zx.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ib.haigaiapp.cn

TS:   [...arr];
来源：http://ax.9csxet.cn

Java: new ArrayList<>(list);
来源：http://tg.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://je.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://pc.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://xd.hahajie.cn

[D23] reduce 累积计算
来源：http://ig.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hq.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pq.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ep.shxzskj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mn.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wu.shxzskj.cn

Go:   // 手写循环
来源：http://yp.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gs.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qf.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://md.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bb.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://am.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xx.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ni.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ds.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://el.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fb.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zh.asd995.cn

[D25] Set 集合去重与交并差
来源：http://zb.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ls.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jv.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yc.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wx.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xj.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hi.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hy.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zz.szsharing.cn

[D26] 数组转字符串
来源：http://fa.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://vw.bookmarksfly.cn

PHP:  implode(", ", $arr);
来源：http://en.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://iw.bjjhwx.cn

TS:   arr.join(", ")
来源：http://aj.gzmigu.cn

Java: String.join(", ", list)
来源：http://pu.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://nr.huanxung.cn

Ruby: arr.join(", ")
来源：http://jk.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://dr.gzmigu.cn

================================================================================
来源：http://qi.chemitech.net.cn

E. 字符串处理
来源：http://mi.bjjhwx.cn

================================================================================
来源：http://si.haigaiapp.cn

[E01] 拼接字符串
来源：http://ul.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gk.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rh.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vq.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hu.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eu.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tt.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vc.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yl.yuntaijiaju.cn

[E02] 重复字符串
来源：http://ej.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://ip.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://xz.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://de.newstarts.cn

TS:   "ab".repeat(3)
来源：http://kr.yuntaijiaju.cn

Java: "ab".repeat(3)
来源：http://dk.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://hl.colortex.cn

Ruby: "ab" * 3
来源：http://kc.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hy.nszjky.cn

[E03] 截取子串
来源：http://ce.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nd.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tc.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nz.nicolike.cn

TS:   s.slice(1, 4)
来源：http://zm.gzmigu.cn

Java: s.substring(1, 4)
来源：http://lj.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ax.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dk.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://xa.szxytkj.cn

[E04] 查找子串位置
来源：http://xt.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://gm.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://wt.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mw.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://qn.lnxyls.cn

Java: s.indexOf("x")
来源：http://gk.asd995.cn

Go:   strings.Index(s, "x")
来源：http://nx.panjiajie.cn

Ruby: s.index("x")
来源：http://ao.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://ab.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xs.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ko.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ji.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://px.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rs.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bv.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uw.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aa.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gj.9csxet.cn

[E06] 替换子串
来源：http://cc.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sj.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://zo.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lb.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://ft.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wd.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dc.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gw.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://kj.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://ke.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ks.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qg.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gb.shxzukj.cn

TS:   s.split(",")
来源：http://gd.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kt.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vz.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://ov.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ch.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://rg.nszjky.cn

Py:   ",".join(items)
来源：http://ov.szxytkj.cn

PHP:  implode(",", $items);
来源：http://ow.colortex.cn

JS:   items.join(",")
来源：http://dx.chemitech.net.cn

TS:   items.join(",")
来源：http://cl.lnxyls.cn

Java: String.join(",", items)
来源：http://gj.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://nw.colortex.cn

Ruby: items.join(",")
来源：http://cl.shxzskj.cn

C#:   string.Join(",", items)
来源：http://tx.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://ja.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tb.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qw.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://mz.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://xl.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://yu.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wc.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hp.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vc.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://ow.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dn.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fb.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://hk.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://ex.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://ct.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://og.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uk.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mt.nszjky.cn

[E11] 反转字符串
来源：http://ws.hnjuh.cn

Py:   s[::-1]
来源：http://qi.shtwfgs.cn

PHP:  strrev($s);
来源：http://zd.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://qp.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://hy.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ix.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://iu.jctech888.com.cn

Ruby: s.reverse
来源：http://wj.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://na.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://yj.shxzukj.cn

Py:   s.count("a")
来源：http://kw.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://ij.nszjky.cn

JS:   s.split("a").length - 1
来源：http://yp.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://sz.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xy.521024.cn

Go:   strings.Count(s, "a")
来源：http://fm.lnxyls.cn

Ruby: s.count("a")
来源：http://bd.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://ga.shxzukj.cn

[E13] 逐字符遍历
来源：http://xu.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://oq.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sd.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pk.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rt.huixiangedu.cn


<!-- 参考信息 -->