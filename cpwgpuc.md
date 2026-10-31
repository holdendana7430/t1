代发 wailian999

Java: list.size();
来源：http://fp.shtwfgs.cn

Go:   len(arr)
来源：http://pr.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://fb.nszjky.cn

C#:   list.Count;
来源：http://lm.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://sx.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qb.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vq.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://hu.haigaiapp.cn

TS:   arr.slice(1, 4);
来源：http://nr.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://zg.hnjuh.cn

Go:   arr[1:4]
来源：http://ef.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://wc.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://fh.asd995.cn

[D08] 合并两个数组
来源：http://qv.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://mj.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://dk.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gl.jctech888.com.cn

TS:   [...a, ...b];
来源：http://au.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vo.colortex.cn

Go:   append(a, b...)
来源：http://fe.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://mr.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://hz.wgjwhj.cn

[D09] 排序（升序）
来源：http://gf.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://kb.colortex.cn

PHP:  sort($arr);
来源：http://iz.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ma.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xd.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rn.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kh.hnjuh.cn

Ruby: arr.sort
来源：http://do.colortex.cn

C#:   list.Sort();
来源：http://zd.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://op.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uu.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rg.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://st.huixiangedu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oe.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vd.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ey.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ag.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jq.huanxung.cn

[D11] 反转数组
来源：http://fi.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://og.huanxung.cn

PHP:  array_reverse($arr);
来源：http://hw.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tp.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://iy.nicolike.cn

Java: Collections.reverse(list);
来源：http://ti.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://ov.chemitech.net.cn

Ruby: arr.reverse
来源：http://lt.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://jk.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://ce.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://hk.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xf.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zo.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qa.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ow.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://pi.panjiajie.cn

Ruby: arr.index(x)
来源：http://kv.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://qj.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://gq.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ld.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ji.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://pv.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://kq.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zv.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ek.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kv.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kg.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://pz.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://io.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ty.bjjhwx.cn

JS:   arr.map(x => x * 2)
来源：http://rw.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://ry.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nx.huixiangedu.cn

Go:   // 手写循环
来源：http://dc.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nk.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ph.szxytkj.cn

[D15] 去重
来源：http://wq.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gh.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://jc.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://kl.huanxung.cn

TS:   [...new Set(arr)]
来源：http://ib.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sn.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jn.huixiangedu.cn

Ruby: arr.uniq
来源：http://eg.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://si.shxzukj.cn

[D16] 求和与平均值
来源：http://rd.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hj.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fm.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ah.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://au.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kp.gzmigu.cn

Go:   // 手写循环累加
来源：http://xj.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fr.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://al.haigaiapp.cn

[D17] 最大值与最小值
来源：http://id.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://cx.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://dj.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ms.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://qn.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rk.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lr.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://uw.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://iw.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://oe.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xy.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://af.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jy.shtwfgs.cn

TS:   nested.flat();
来源：http://ay.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cd.jctech888.com.cn

Go:   // 手写双层循环
来源：http://on.nicolike.cn

Ruby: nested.flatten
来源：http://ty.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ry.shxzukj.cn

[D19] 按字段分组
来源：http://la.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ex.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gx.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lc.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ap.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fy.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://bi.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zo.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qx.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://as.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://ar.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://hn.wgjwhj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bp.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ph.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dt.nszjky.cn

Go:   // 手写 map[T]int
来源：http://my.hnjuh.cn

Ruby: arr.tally
来源：http://is.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gn.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://zm.huanxung.cn

Py:   x in arr
来源：http://nw.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://kb.chemitech.net.cn

JS:   arr.includes(x)
来源：http://gg.shxzskj.cn

TS:   arr.includes(x)
来源：http://zc.wgjwhj.cn

Java: list.contains(x)
来源：http://ap.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://hv.nszjky.cn

Ruby: arr.include?(x)
来源：http://kv.bjjhwx.cn

C#:   list.Contains(x)
来源：http://bs.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://ov.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dj.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ay.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ir.jianghongdianzi.cn

TS:   [...arr];
来源：http://pz.newstarts.cn

Java: new ArrayList<>(list);
来源：http://uo.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vc.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://mv.nszjky.cn

C#:   new List<int>(list);
来源：http://vt.asd995.cn

[D23] reduce 累积计算
来源：http://og.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tx.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pc.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vh.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yo.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bh.colortex.cn

Go:   // 手写循环
来源：http://uu.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://na.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ll.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://pf.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sc.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kf.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wm.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tu.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yn.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wr.hnjuh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ge.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sk.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://hk.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dl.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pd.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zx.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qa.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ve.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://md.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gv.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xb.shxzskj.cn

[D26] 数组转字符串
来源：http://eh.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://kv.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://oo.gzmigu.cn

JS:   arr.join(", ")
来源：http://zl.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://iw.colortex.cn

Java: String.join(", ", list)
来源：http://wm.hahajie.cn

Go:   strings.Join(strs, ", ")
来源：http://ht.panjiajie.cn

Ruby: arr.join(", ")
来源：http://um.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://sm.hnjuh.cn

================================================================================
来源：http://by.haigaiapp.cn

E. 字符串处理
来源：http://at.huixiangedu.cn

================================================================================
来源：http://nz.wgjwhj.cn

[E01] 拼接字符串
来源：http://py.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://px.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rt.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://um.jianghongdianzi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kd.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qx.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ry.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sn.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ye.yuexingan06.cn

[E02] 重复字符串
来源：http://oq.muxihuayi.cn

Py:   "ab" * 3
来源：http://oy.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://pn.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://ai.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://bk.nszjky.cn

Java: "ab".repeat(3)
来源：http://qw.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://et.9csxet.cn

Ruby: "ab" * 3
来源：http://bu.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qz.yuexingan06.cn

[E03] 截取子串
来源：http://qh.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pl.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ea.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pm.9csxet.cn

TS:   s.slice(1, 4)
来源：http://cp.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://vd.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://me.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mb.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://he.bjjhwx.cn

[E04] 查找子串位置
来源：http://zv.asd995.cn

Py:   s.find("x");  s.index("x")
来源：http://co.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://ol.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mu.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://ft.szxytkj.cn

Java: s.indexOf("x")
来源：http://wp.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://ty.shxzukj.cn

Ruby: s.index("x")
来源：http://nl.521024.cn

C#:   s.IndexOf("x")
来源：http://hc.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pg.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://at.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kn.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gh.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eu.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qh.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dk.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hm.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gm.yuexingan06.cn

[E06] 替换子串
来源：http://vv.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ta.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://jv.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mu.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://fv.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kx.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qp.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mj.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://mv.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://hm.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wk.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vf.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://am.bjjhwx.cn

TS:   s.split(",")
来源：http://gq.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jy.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dj.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://mi.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vd.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://qp.9csxet.cn

Py:   ",".join(items)
来源：http://ye.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://se.lnxyls.cn

JS:   items.join(",")
来源：http://kc.colortex.cn

TS:   items.join(",")
来源：http://pz.jctech888.com.cn

Java: String.join(",", items)
来源：http://dq.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://gd.huanxung.cn

Ruby: items.join(",")
来源：http://nq.gzmigu.cn

C#:   string.Join(",", items)
来源：http://ng.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://ea.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ru.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ig.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://el.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://tv.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://db.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ry.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dm.huixiangedu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ud.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://ax.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rz.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ez.newstarts.cn

JS:   "7".padStart(3, "0")
来源：http://hg.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://zi.hahajie.cn

Java: String.format("%03d", 7)
来源：http://gf.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tg.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hr.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vu.jianghongdianzi.cn

[E11] 反转字符串
来源：http://va.panjiajie.cn

Py:   s[::-1]
来源：http://ie.szsharing.cn

PHP:  strrev($s);
来源：http://tn.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://mo.asd995.cn

TS:   [...s].reverse().join("")
来源：http://qk.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vu.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jb.jianghongdianzi.cn

Ruby: s.reverse
来源：http://ly.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pi.bjjhwx.cn

[E12] 统计某字符出现次数
来源：http://wk.jianghongdianzi.cn

Py:   s.count("a")
来源：http://rh.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://lt.hahajie.cn

JS:   s.split("a").length - 1
来源：http://im.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://go.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xq.asd995.cn

Go:   strings.Count(s, "a")
来源：http://hd.asd995.cn

Ruby: s.count("a")
来源：http://cp.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://so.hnjuh.cn

[E13] 逐字符遍历
来源：http://vq.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://mi.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xa.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tf.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xk.shxzukj.cn


<!-- 参考信息 -->