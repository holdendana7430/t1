代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://yn.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://dw.chemitech.net.cn

[D09] 排序（升序）
来源：http://ck.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://dt.hnjuh.cn

PHP:  sort($arr);
来源：http://nw.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://us.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bi.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yv.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cz.521024.cn

Ruby: arr.sort
来源：http://nb.huixinmuqiang.cn

C#:   list.Sort();
来源：http://nl.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zd.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mu.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fj.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ai.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gu.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mb.lnxyls.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zp.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qc.jianghongdianzi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ws.hnjuh.cn

[D11] 反转数组
来源：http://gw.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qi.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://tb.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nt.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://rc.colortex.cn

Java: Collections.reverse(list);
来源：http://fq.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://gu.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://gz.521024.cn

C#:   list.Reverse();
来源：http://lh.huanxung.cn

[D12] 查找元素下标
来源：http://qo.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://tk.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://so.nszjky.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vn.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hs.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vm.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://wp.muxihuayi.cn

Ruby: arr.index(x)
来源：http://js.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://vm.nszjky.cn

[D13] 过滤（保留满足条件的）
来源：http://un.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ay.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ua.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://vx.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://dz.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nl.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dd.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fg.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zt.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://bu.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cy.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tf.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://my.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://wx.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yn.szxytkj.cn

Go:   // 手写循环
来源：http://oa.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nc.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ov.shtwfgs.cn

[D15] 去重
来源：http://td.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yy.hnjuh.cn

PHP:  array_unique($arr);
来源：http://iw.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://pk.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://pq.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://os.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zo.chemitech.net.cn

Ruby: arr.uniq
来源：http://vc.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://cl.colortex.cn

[D16] 求和与平均值
来源：http://rx.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hs.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ff.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hq.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ru.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sg.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://ct.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jo.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://ax.asd995.cn

[D17] 最大值与最小值
来源：http://vb.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://nt.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://oo.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bl.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://mk.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jk.521024.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hw.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://vt.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://sc.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://eq.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tm.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://rk.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gz.yuntaijiaju.cn

TS:   nested.flat();
来源：http://nd.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gt.bjjhwx.cn

Go:   // 手写双层循环
来源：http://ap.hnjuh.cn

Ruby: nested.flatten
来源：http://sb.szsharing.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yq.bjjhwx.cn

[D19] 按字段分组
来源：http://po.bjjhwx.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vy.bookmarksfly.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ru.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dv.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cx.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vr.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://rc.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gt.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ws.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://qm.bjjhwx.cn

Py:   Counter(arr)
来源：http://nk.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://op.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dz.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zb.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kt.9csxet.cn

Go:   // 手写 map[T]int
来源：http://av.wgjwhj.cn

Ruby: arr.tally
来源：http://fa.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://us.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://tb.huixinmuqiang.cn

Py:   x in arr
来源：http://xr.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://cm.shtwfgs.cn

JS:   arr.includes(x)
来源：http://ia.asd995.cn

TS:   arr.includes(x)
来源：http://lu.shtwfgs.cn

Java: list.contains(x)
来源：http://pi.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://ir.szxytkj.cn

Ruby: arr.include?(x)
来源：http://ou.panjiajie.cn

C#:   list.Contains(x)
来源：http://ro.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://pb.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ht.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rj.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bg.newstarts.cn

TS:   [...arr];
来源：http://aq.nicolike.cn

Java: new ArrayList<>(list);
来源：http://xe.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rj.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://az.szsharing.cn

C#:   new List<int>(list);
来源：http://jf.wgjwhj.cn

[D23] reduce 累积计算
来源：http://yy.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rn.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yw.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://et.muxihuayi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rq.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lf.bjjhwx.cn

Go:   // 手写循环
来源：http://wf.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uu.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lk.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://ne.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ir.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://om.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pr.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ua.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sn.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mc.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ql.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yh.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://ae.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yr.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uo.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hh.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wp.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zt.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nq.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ed.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xt.szxytkj.cn

[D26] 数组转字符串
来源：http://pb.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://sl.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://tf.hnjuh.cn

JS:   arr.join(", ")
来源：http://wh.shtwfgs.cn

TS:   arr.join(", ")
来源：http://ll.yuexingan06.cn

Java: String.join(", ", list)
来源：http://ce.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://xk.panjiajie.cn

Ruby: arr.join(", ")
来源：http://ux.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://dj.huanxung.cn

================================================================================
来源：http://vh.szsharing.cn

E. 字符串处理
来源：http://xu.shtwfgs.cn

================================================================================
来源：http://ma.colortex.cn

[E01] 拼接字符串
来源：http://by.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gk.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vm.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mm.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gx.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bt.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ps.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jk.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ko.szxytkj.cn

[E02] 重复字符串
来源：http://cv.lnxyls.cn

Py:   "ab" * 3
来源：http://gh.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://mm.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://xw.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://vd.9csxet.cn

Java: "ab".repeat(3)
来源：http://sz.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://cv.panjiajie.cn

Ruby: "ab" * 3
来源：http://ff.colortex.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iz.panjiajie.cn

[E03] 截取子串
来源：http://ys.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kt.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gm.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://as.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://tz.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://qt.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ue.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zd.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://xx.yuexingan06.cn

[E04] 查找子串位置
来源：http://ln.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://ao.9csxet.cn

PHP:  strpos($s, "x");
来源：http://yb.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jt.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://jx.521024.cn

Java: s.indexOf("x")
来源：http://mw.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://ww.huixiangedu.cn

Ruby: s.index("x")
来源：http://qf.hahajie.cn

C#:   s.IndexOf("x")
来源：http://pj.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dd.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mj.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ig.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://he.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tr.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jx.nicolike.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gl.hnjuh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://el.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rs.hnjuh.cn

[E06] 替换子串
来源：http://ju.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cc.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://hg.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xz.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://wc.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jo.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xs.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vc.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://vi.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://ce.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ir.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mk.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://uw.521024.cn

TS:   s.split(",")
来源：http://ii.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vp.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fr.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://rw.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://we.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://us.chemitech.net.cn

Py:   ",".join(items)
来源：http://em.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://et.jctech888.com.cn

JS:   items.join(",")
来源：http://dr.haigaiapp.cn

TS:   items.join(",")
来源：http://cb.bjjhwx.cn

Java: String.join(",", items)
来源：http://lk.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://ux.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://uh.huanxung.cn

C#:   string.Join(",", items)
来源：http://iz.gzmigu.cn

[E09] 去除所有空白字符
来源：http://nu.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xj.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rj.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://ot.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://qr.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://hs.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sp.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xs.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bl.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://fp.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ov.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sk.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://gt.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://pc.hahajie.cn

Java: String.format("%03d", 7)
来源：http://li.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pf.colortex.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hs.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dp.jctech888.com.cn

[E11] 反转字符串
来源：http://sr.shtwfgs.cn

Py:   s[::-1]
来源：http://mj.nicolike.cn

PHP:  strrev($s);
来源：http://qr.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://nu.521024.cn

TS:   [...s].reverse().join("")
来源：http://ue.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ff.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kz.bookmarksfly.cn

Ruby: s.reverse
来源：http://kz.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nj.asd995.cn

[E12] 统计某字符出现次数
来源：http://xg.nicolike.cn

Py:   s.count("a")
来源：http://bq.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://vl.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://ht.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://ph.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://of.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://rg.shxzskj.cn

Ruby: s.count("a")
来源：http://mt.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://bn.panjiajie.cn

[E13] 逐字符遍历
来源：http://kn.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://ix.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ca.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yv.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dw.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ad.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ie.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lo.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://st.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://ks.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fx.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uw.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ck.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tw.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zi.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ra.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sh.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://os.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://kg.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jo.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jr.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ul.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dv.wgjwhj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ma.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ty.nszjky.cn


<!-- 参考信息 -->