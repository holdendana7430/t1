代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://cc.huixiangedu.cn

[D08] 合并两个数组
来源：http://sv.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://uh.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://kj.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fg.hnjuh.cn

TS:   [...a, ...b];
来源：http://bi.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://up.huixiangedu.cn

Go:   append(a, b...)
来源：http://fh.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://dl.wgjwhj.cn

C#:   a.Concat(b).ToList()
来源：http://lf.panjiajie.cn

[D09] 排序（升序）
来源：http://uj.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://vw.szxytkj.cn

PHP:  sort($arr);
来源：http://zd.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vt.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://va.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://as.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vw.hahajie.cn

Ruby: arr.sort
来源：http://rm.hahajie.cn

C#:   list.Sort();
来源：http://ok.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://od.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wx.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kg.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mw.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qr.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cq.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ex.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hy.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dq.huixiangedu.cn

[D11] 反转数组
来源：http://pf.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gp.9csxet.cn

PHP:  array_reverse($arr);
来源：http://bg.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tj.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://ub.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://ub.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://ki.shxzukj.cn

Ruby: arr.reverse
来源：http://gl.nicolike.cn

C#:   list.Reverse();
来源：http://kl.asd995.cn

[D12] 查找元素下标
来源：http://vh.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://fi.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uu.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cm.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ct.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jo.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://nb.hnjuh.cn

Ruby: arr.index(x)
来源：http://ry.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://ks.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://ps.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bh.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wf.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://wb.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://aw.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zy.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ra.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://br.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nk.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://br.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rj.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zf.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://zo.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://tq.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hv.panjiajie.cn

Go:   // 手写循环
来源：http://ew.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lj.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hp.nszjky.cn

[D15] 去重
来源：http://ue.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mq.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://fv.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://zr.colortex.cn

TS:   [...new Set(arr)]
来源：http://kw.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kw.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zl.bjjhwx.cn

Ruby: arr.uniq
来源：http://ow.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://tb.hnjuh.cn

[D16] 求和与平均值
来源：http://nk.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lx.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mi.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xl.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kp.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pl.nicolike.cn

Go:   // 手写循环累加
来源：http://ml.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pz.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://hl.gzmigu.cn

[D17] 最大值与最小值
来源：http://ms.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://hh.521024.cn

PHP:  max($arr);  min($arr);
来源：http://nh.nszjky.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uu.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://pd.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hg.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wd.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://go.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://tg.colortex.cn

[D18] 扁平化嵌套数组
来源：http://uy.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iy.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://zq.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://et.jianghongdianzi.cn

TS:   nested.flat();
来源：http://fc.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cz.wgjwhj.cn

Go:   // 手写双层循环
来源：http://kh.nicolike.cn

Ruby: nested.flatten
来源：http://kx.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bc.szsharing.cn

[D19] 按字段分组
来源：http://oh.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ew.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ig.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://au.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ka.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gm.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://sk.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nj.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gw.asd995.cn

[D20] 统计每个元素出现次数
来源：http://ty.newstarts.cn

Py:   Counter(arr)
来源：http://mk.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://ec.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ph.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dm.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jl.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://gi.szsharing.cn

Ruby: arr.tally
来源：http://zu.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dd.nicolike.cn

[D21] 判断是否包含某元素
来源：http://ss.jianghongdianzi.cn

Py:   x in arr
来源：http://nx.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://wn.jctech888.com.cn

JS:   arr.includes(x)
来源：http://qj.gzmigu.cn

TS:   arr.includes(x)
来源：http://mx.hnjuh.cn

Java: list.contains(x)
来源：http://lv.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://yy.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://tl.szxytkj.cn

C#:   list.Contains(x)
来源：http://jd.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://ms.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mo.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lg.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://si.hnjuh.cn

TS:   [...arr];
来源：http://tk.9csxet.cn

Java: new ArrayList<>(list);
来源：http://gj.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ez.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://wj.bjjhwx.cn

C#:   new List<int>(list);
来源：http://lu.shxzukj.cn

[D23] reduce 累积计算
来源：http://qv.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kf.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fg.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nx.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bd.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kx.gzmigu.cn

Go:   // 手写循环
来源：http://gb.haigaiapp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ai.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yt.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://ht.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://co.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oj.huixinmuqiang.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lz.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jt.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yi.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zo.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://an.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yj.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://qv.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ol.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://os.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fp.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bk.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kg.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mo.shxzukj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zj.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ew.bookmarksfly.cn

[D26] 数组转字符串
来源：http://cn.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://ex.colortex.cn

PHP:  implode(", ", $arr);
来源：http://lf.nszjky.cn

JS:   arr.join(", ")
来源：http://jw.szxytkj.cn

TS:   arr.join(", ")
来源：http://ts.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://kq.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://qb.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://dl.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://bp.gzmigu.cn

================================================================================
来源：http://xt.panjiajie.cn

E. 字符串处理
来源：http://jy.9csxet.cn

================================================================================
来源：http://mq.asd995.cn

[E01] 拼接字符串
来源：http://jq.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hb.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fs.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://le.jianghongdianzi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rs.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cm.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sh.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ve.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oz.newstarts.cn

[E02] 重复字符串
来源：http://lm.panjiajie.cn

Py:   "ab" * 3
来源：http://ra.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://jd.colortex.cn

JS:   "ab".repeat(3)
来源：http://hb.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://nr.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://ar.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://wl.panjiajie.cn

Ruby: "ab" * 3
来源：http://mn.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cz.lnxyls.cn

[E03] 截取子串
来源：http://sv.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ev.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wb.gzmigu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wc.nszjky.cn

TS:   s.slice(1, 4)
来源：http://pt.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://ij.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uk.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vh.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://by.asd995.cn

[E04] 查找子串位置
来源：http://jt.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://ej.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://au.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mb.huanxung.cn

TS:   s.indexOf("x")
来源：http://xf.colortex.cn

Java: s.indexOf("x")
来源：http://xx.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://xy.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://xg.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://vt.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tt.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vn.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ou.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lw.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xf.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gc.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yw.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tx.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dy.huixiangedu.cn

[E06] 替换子串
来源：http://gr.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ie.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://jq.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mt.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://gg.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uz.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oq.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ua.asd995.cn

C#:   s.Replace("a", "b")
来源：http://ng.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://bs.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ra.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eq.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gy.haigaiapp.cn

TS:   s.split(",")
来源：http://wh.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fi.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jf.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://na.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tk.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://fn.szsharing.cn

Py:   ",".join(items)
来源：http://qg.asd995.cn

PHP:  implode(",", $items);
来源：http://ac.muxihuayi.cn

JS:   items.join(",")
来源：http://kn.huixinmuqiang.cn

TS:   items.join(",")
来源：http://vs.hnjuh.cn

Java: String.join(",", items)
来源：http://ok.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://jx.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://sl.newstarts.cn

C#:   string.Join(",", items)
来源：http://dv.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://mo.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fj.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://te.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://zl.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://md.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://yz.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zj.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qz.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cm.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://ya.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fh.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zr.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://fw.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://uc.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://sb.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://oi.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rd.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ts.jctech888.com.cn

[E11] 反转字符串
来源：http://oz.521024.cn

Py:   s[::-1]
来源：http://gl.huixiangedu.cn

PHP:  strrev($s);
来源：http://rm.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://ds.521024.cn

TS:   [...s].reverse().join("")
来源：http://fz.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xl.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jl.nszjky.cn

Ruby: s.reverse
来源：http://hn.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bs.9csxet.cn

[E12] 统计某字符出现次数
来源：http://sm.panjiajie.cn

Py:   s.count("a")
来源：http://lq.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://yt.huanxung.cn

JS:   s.split("a").length - 1
来源：http://nc.hahajie.cn

TS:   s.split("a").length - 1
来源：http://sh.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yg.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://kh.shxzukj.cn

Ruby: s.count("a")
来源：http://vm.shtwfgs.cn

C#:   s.Count(c => c == 'a')
来源：http://rr.szsharing.cn

[E13] 逐字符遍历
来源：http://pe.asd995.cn

Py:   for ch in s: print(ch)
来源：http://of.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://im.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vm.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dx.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fh.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cm.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ff.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://px.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://rr.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sv.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kf.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bp.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ph.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ub.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ej.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rn.nicolike.cn


<!-- 参考信息 -->