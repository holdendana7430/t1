代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://op.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://ks.huixiangedu.cn

[D09] 排序（升序）
来源：http://py.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://xf.nszjky.cn

PHP:  sort($arr);
来源：http://zy.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bq.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jd.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qt.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bk.shxzukj.cn

Ruby: arr.sort
来源：http://za.haigaiapp.cn

C#:   list.Sort();
来源：http://of.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ga.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hf.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nm.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lk.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mi.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oj.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://au.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tj.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dc.yuexingan06.cn

[D11] 反转数组
来源：http://lp.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wr.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://ud.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nj.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://rn.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://dj.521024.cn

Go:   slices.Reverse(arr)
来源：http://ym.yuexingan06.cn

Ruby: arr.reverse
来源：http://ko.szsharing.cn

C#:   list.Reverse();
来源：http://zn.szsharing.cn

[D12] 查找元素下标
来源：http://yg.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://rv.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vv.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hk.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://we.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mw.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://zs.shxzskj.cn

Ruby: arr.index(x)
来源：http://cw.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://ch.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://ng.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gu.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mn.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://zm.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://pz.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ww.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mp.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://et.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ke.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://qr.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nn.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vg.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://ii.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://ad.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tm.bjjhwx.cn

Go:   // 手写循环
来源：http://ml.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://um.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sx.521024.cn

[D15] 去重
来源：http://rg.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ox.hnjuh.cn

PHP:  array_unique($arr);
来源：http://tn.521024.cn

JS:   [...new Set(arr)]
来源：http://hp.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://fw.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kx.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uc.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://rj.asd995.cn

C#:   list.Distinct().ToList()
来源：http://if.jctech888.com.cn

[D16] 求和与平均值
来源：http://js.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ec.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nn.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vq.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wf.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://er.huixiangedu.cn

Go:   // 手写循环累加
来源：http://gs.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://it.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://dn.hahajie.cn

[D17] 最大值与最小值
来源：http://gz.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://mf.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://bc.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iz.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://mf.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xj.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://av.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://ej.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://cv.asd995.cn

[D18] 扁平化嵌套数组
来源：http://jk.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oa.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://li.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://td.lnxyls.cn

TS:   nested.flat();
来源：http://qt.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pz.szxytkj.cn

Go:   // 手写双层循环
来源：http://ie.gzmigu.cn

Ruby: nested.flatten
来源：http://op.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kj.asd995.cn

[D19] 按字段分组
来源：http://jv.newstarts.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rh.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ej.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://py.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yb.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kw.521024.cn

Go:   // 手写 map[string][]T
来源：http://in.hnjuh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yf.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://km.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://zl.panjiajie.cn

Py:   Counter(arr)
来源：http://st.huanxung.cn

PHP:  array_count_values($arr);
来源：http://mo.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://di.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cg.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zc.nszjky.cn

Go:   // 手写 map[T]int
来源：http://jz.hnjuh.cn

Ruby: arr.tally
来源：http://mg.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mb.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://au.panjiajie.cn

Py:   x in arr
来源：http://rz.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://pm.muxihuayi.cn

JS:   arr.includes(x)
来源：http://oa.521024.cn

TS:   arr.includes(x)
来源：http://rr.huixinmuqiang.cn

Java: list.contains(x)
来源：http://zw.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://uo.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://bl.wgjwhj.cn

C#:   list.Contains(x)
来源：http://cg.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://bl.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ke.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ob.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ui.huanxung.cn

TS:   [...arr];
来源：http://gj.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://yv.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mt.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://me.lnxyls.cn

C#:   new List<int>(list);
来源：http://gh.wgjwhj.cn

[D23] reduce 累积计算
来源：http://el.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://df.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ev.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fa.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://je.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ww.szsharing.cn

Go:   // 手写循环
来源：http://fc.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sl.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hn.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://xo.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fa.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://my.huixinmuqiang.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xd.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yi.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hx.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yv.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uq.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oa.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://xb.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ug.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gi.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://id.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rf.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ax.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sk.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nn.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ua.jctech888.com.cn

[D26] 数组转字符串
来源：http://tq.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://ud.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://qu.shxzskj.cn

JS:   arr.join(", ")
来源：http://ux.9csxet.cn

TS:   arr.join(", ")
来源：http://xk.wgjwhj.cn

Java: String.join(", ", list)
来源：http://rg.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://un.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://mx.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://la.jianghongdianzi.cn

================================================================================
来源：http://xf.huixiangedu.cn

E. 字符串处理
来源：http://ci.huanxung.cn

================================================================================
来源：http://nx.bookmarksfly.cn

[E01] 拼接字符串
来源：http://um.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fz.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://td.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ip.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lq.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vd.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kb.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cl.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qo.shtwfgs.cn

[E02] 重复字符串
来源：http://qh.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://uu.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://qn.huanxung.cn

JS:   "ab".repeat(3)
来源：http://lq.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://jc.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://oe.wgjwhj.cn

Go:   strings.Repeat("ab", 3)
来源：http://lr.nicolike.cn

Ruby: "ab" * 3
来源：http://ke.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ep.hahajie.cn

[E03] 截取子串
来源：http://rc.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cm.jianghongdianzi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vp.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ge.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://va.huanxung.cn

Java: s.substring(1, 4)
来源：http://lt.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://er.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://aw.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://ob.szsharing.cn

[E04] 查找子串位置
来源：http://gx.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://bj.hahajie.cn

PHP:  strpos($s, "x");
来源：http://lq.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yq.9csxet.cn

TS:   s.indexOf("x")
来源：http://pt.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://vb.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://ux.yuexingan06.cn

Ruby: s.index("x")
来源：http://ds.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://or.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://op.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pd.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jd.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://da.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yt.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pl.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://os.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uo.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rs.asd995.cn

[E06] 替换子串
来源：http://pi.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dv.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://of.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cw.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://ti.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://in.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ar.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uz.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://ph.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://bn.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tj.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mz.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kw.lnxyls.cn

TS:   s.split(",")
来源：http://fm.gzmigu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xs.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://br.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://ur.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pz.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://nv.huanxung.cn

Py:   ",".join(items)
来源：http://if.panjiajie.cn

PHP:  implode(",", $items);
来源：http://gy.huixinmuqiang.cn

JS:   items.join(",")
来源：http://ud.szxytkj.cn

TS:   items.join(",")
来源：http://oy.hahajie.cn

Java: String.join(",", items)
来源：http://oi.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://hn.szsharing.cn

Ruby: items.join(",")
来源：http://ev.9csxet.cn

C#:   string.Join(",", items)
来源：http://wu.huanxung.cn

[E09] 去除所有空白字符
来源：http://uh.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rf.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wx.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://cr.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://hc.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://mq.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xw.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oh.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uh.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://qh.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ea.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ls.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://im.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://gb.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://mm.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ex.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zj.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hj.bjjhwx.cn

[E11] 反转字符串
来源：http://ti.bjjhwx.cn

Py:   s[::-1]
来源：http://ri.panjiajie.cn

PHP:  strrev($s);
来源：http://io.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://hs.colortex.cn

TS:   [...s].reverse().join("")
来源：http://hd.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cv.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ml.hnjuh.cn

Ruby: s.reverse
来源：http://ed.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cb.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://bs.lnxyls.cn

Py:   s.count("a")
来源：http://kg.asd995.cn

PHP:  substr_count($s, "a");
来源：http://pm.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://mv.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://jt.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jg.asd995.cn

Go:   strings.Count(s, "a")
来源：http://pj.nszjky.cn

Ruby: s.count("a")
来源：http://xn.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://lq.521024.cn

[E13] 逐字符遍历
来源：http://ek.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://ni.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ea.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ee.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://su.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mz.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dl.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wi.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cr.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://pq.hahajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ry.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ap.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://px.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ae.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cl.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iq.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://az.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sf.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://yt.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ev.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gb.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gw.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ox.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zu.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://at.shtwfgs.cn


<!-- 参考信息 -->