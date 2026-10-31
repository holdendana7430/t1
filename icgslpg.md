代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://yt.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://pj.lnxyls.cn

[D09] 排序（升序）
来源：http://mu.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://gk.huanxung.cn

PHP:  sort($arr);
来源：http://tj.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zk.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kn.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lw.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cx.szsharing.cn

Ruby: arr.sort
来源：http://su.haigaiapp.cn

C#:   list.Sort();
来源：http://tw.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ss.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ib.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qd.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yz.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yj.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wc.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ve.shtwfgs.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ed.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vx.521024.cn

[D11] 反转数组
来源：http://sh.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://im.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://xt.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hc.gzmigu.cn

TS:   [...arr].reverse();
来源：http://ml.lnxyls.cn

Java: Collections.reverse(list);
来源：http://vw.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://kj.nszjky.cn

Ruby: arr.reverse
来源：http://sm.szxytkj.cn

C#:   list.Reverse();
来源：http://fb.9csxet.cn

[D12] 查找元素下标
来源：http://xj.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://ol.newstarts.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gx.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ji.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bi.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ob.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://xg.muxihuayi.cn

Ruby: arr.index(x)
来源：http://ea.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://go.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://cg.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://le.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zs.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://ic.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://wa.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lw.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ot.nicolike.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wm.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ug.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://uy.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yw.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jm.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://pf.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://oa.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jf.bjjhwx.cn

Go:   // 手写循环
来源：http://xa.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://iy.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xc.asd995.cn

[D15] 去重
来源：http://mi.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gb.huanxung.cn

PHP:  array_unique($arr);
来源：http://cv.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://zs.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://et.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uw.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ay.muxihuayi.cn

Ruby: arr.uniq
来源：http://yu.colortex.cn

C#:   list.Distinct().ToList()
来源：http://wx.colortex.cn

[D16] 求和与平均值
来源：http://kz.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nq.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fe.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tw.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qo.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://by.newstarts.cn

Go:   // 手写循环累加
来源：http://hz.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hw.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://rq.hnjuh.cn

[D17] 最大值与最小值
来源：http://mg.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://cf.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://zl.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cr.gzmigu.cn

TS:   Math.max(...arr);
来源：http://og.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gk.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rh.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://ch.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://fc.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://jp.muxihuayi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sm.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://ky.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lm.huanxung.cn

TS:   nested.flat();
来源：http://vt.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fx.colortex.cn

Go:   // 手写双层循环
来源：http://ys.shtwfgs.cn

Ruby: nested.flatten
来源：http://wa.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pz.asd995.cn

[D19] 按字段分组
来源：http://pv.bjjhwx.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://df.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://an.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://te.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://il.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vh.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://cw.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mw.yuntaijiaju.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eg.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://wm.9csxet.cn

Py:   Counter(arr)
来源：http://op.nicolike.cn

PHP:  array_count_values($arr);
来源：http://br.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ue.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eq.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://am.hahajie.cn

Go:   // 手写 map[T]int
来源：http://cf.szxytkj.cn

Ruby: arr.tally
来源：http://ol.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wl.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://sc.wgjwhj.cn

Py:   x in arr
来源：http://ab.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://wc.shxzskj.cn

JS:   arr.includes(x)
来源：http://fc.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://co.shtwfgs.cn

Java: list.contains(x)
来源：http://xd.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://oh.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://lz.hnjuh.cn

C#:   list.Contains(x)
来源：http://qn.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://zu.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ed.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ua.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ep.szxytkj.cn

TS:   [...arr];
来源：http://bu.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://kd.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hv.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://cj.newstarts.cn

C#:   new List<int>(list);
来源：http://tb.9csxet.cn

[D23] reduce 累积计算
来源：http://vy.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mx.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nq.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rg.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xr.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vy.muxihuayi.cn

Go:   // 手写循环
来源：http://ug.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yo.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pk.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://kw.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jm.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yg.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ro.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gl.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ae.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mw.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bu.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xx.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://br.chemitech.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uu.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rr.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fs.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ln.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hk.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ay.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ba.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oe.hnjuh.cn

[D26] 数组转字符串
来源：http://nu.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://bp.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://tp.szxytkj.cn

JS:   arr.join(", ")
来源：http://qo.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://os.panjiajie.cn

Java: String.join(", ", list)
来源：http://qw.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://rs.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://iz.huanxung.cn

C#:   string.Join(", ", list)
来源：http://bb.shxzskj.cn

================================================================================
来源：http://fb.hnjuh.cn

E. 字符串处理
来源：http://br.jianghongdianzi.cn

================================================================================
来源：http://li.haigaiapp.cn

[E01] 拼接字符串
来源：http://bf.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ps.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ak.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zu.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ia.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fh.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mj.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ti.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fk.panjiajie.cn

[E02] 重复字符串
来源：http://gi.bookmarksfly.cn

Py:   "ab" * 3
来源：http://bg.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://bf.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://fz.chemitech.net.cn

TS:   "ab".repeat(3)
来源：http://ao.shxzukj.cn

Java: "ab".repeat(3)
来源：http://qy.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://cl.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://ki.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bv.muxihuayi.cn

[E03] 截取子串
来源：http://xu.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nb.panjiajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rz.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fj.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://yi.nicolike.cn

Java: s.substring(1, 4)
来源：http://yi.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nu.asd995.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dx.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://ca.hahajie.cn

[E04] 查找子串位置
来源：http://tv.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://ld.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://kp.newstarts.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tu.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://be.yuexingan06.cn

Java: s.indexOf("x")
来源：http://cg.asd995.cn

Go:   strings.Index(s, "x")
来源：http://ps.colortex.cn

Ruby: s.index("x")
来源：http://tj.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://ju.asd995.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wp.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nn.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zp.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://co.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wi.yuntaijiaju.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://au.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gs.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iz.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ix.huixiangedu.cn

[E06] 替换子串
来源：http://ph.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sd.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://kh.nszjky.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hd.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://tn.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ue.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zh.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sg.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://gl.nszjky.cn

[E07] 按分隔符拆分
来源：http://uz.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wf.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pr.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ab.newstarts.cn

TS:   s.split(",")
来源：http://yp.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fi.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dt.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://wv.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lz.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://vz.colortex.cn

Py:   ",".join(items)
来源：http://hb.asd995.cn

PHP:  implode(",", $items);
来源：http://rj.bjjhwx.cn

JS:   items.join(",")
来源：http://qv.szxytkj.cn

TS:   items.join(",")
来源：http://cc.shxzskj.cn

Java: String.join(",", items)
来源：http://uu.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://bc.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://cf.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://zx.colortex.cn

[E09] 去除所有空白字符
来源：http://fk.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ac.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cy.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://kn.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://cx.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://qb.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rj.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pv.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://my.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://dq.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ab.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xg.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://uz.hnjuh.cn

TS:   "7".padStart(3, "0")
来源：http://me.newstarts.cn

Java: String.format("%03d", 7)
来源：http://pz.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ch.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jg.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mr.szxytkj.cn

[E11] 反转字符串
来源：http://jv.bookmarksfly.cn

Py:   s[::-1]
来源：http://mo.hahajie.cn

PHP:  strrev($s);
来源：http://hp.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://on.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://io.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fs.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ru.521024.cn

Ruby: s.reverse
来源：http://qe.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zv.asd995.cn

[E12] 统计某字符出现次数
来源：http://qi.chemitech.net.cn

Py:   s.count("a")
来源：http://xk.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://bo.nszjky.cn

JS:   s.split("a").length - 1
来源：http://fn.szsharing.cn

TS:   s.split("a").length - 1
来源：http://cw.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kj.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://du.nszjky.cn

Ruby: s.count("a")
来源：http://uv.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://iu.bjjhwx.cn

[E13] 逐字符遍历
来源：http://na.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://ro.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pv.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zv.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fu.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fr.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fm.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://re.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bi.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://de.panjiajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ds.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sb.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ns.colortex.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lp.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fo.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://na.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xm.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bs.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://nw.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://el.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://en.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://op.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://js.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zp.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gi.shtwfgs.cn


<!-- 参考信息 -->