代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ul.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xb.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uy.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eu.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mj.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hj.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://by.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ms.shxzukj.cn

[D11] 反转数组
来源：http://ev.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zp.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://tm.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yh.szsharing.cn

TS:   [...arr].reverse();
来源：http://he.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://yh.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://fz.lnxyls.cn

Ruby: arr.reverse
来源：http://xd.shxzukj.cn

C#:   list.Reverse();
来源：http://qc.jctech888.com.cn

[D12] 查找元素下标
来源：http://xr.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://gc.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bv.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rr.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bw.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ub.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://qf.colortex.cn

Ruby: arr.index(x)
来源：http://sy.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://nz.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://zr.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fr.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vw.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://mc.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://pk.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xu.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gw.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gu.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bp.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://zy.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://my.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://av.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://cm.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://xe.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ko.huixinmuqiang.cn

Go:   // 手写循环
来源：http://dc.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pv.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qh.bjjhwx.cn

[D15] 去重
来源：http://xy.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://de.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://go.szsharing.cn

JS:   [...new Set(arr)]
来源：http://ta.huanxung.cn

TS:   [...new Set(arr)]
来源：http://jr.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wa.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fw.shxzskj.cn

Ruby: arr.uniq
来源：http://af.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://ij.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://hf.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xv.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nc.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ya.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ny.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pl.colortex.cn

Go:   // 手写循环累加
来源：http://dl.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://av.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://hc.panjiajie.cn

[D17] 最大值与最小值
来源：http://fw.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://wp.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://yo.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hy.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://yj.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xg.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://si.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://ak.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://nr.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://tw.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ry.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://qu.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kq.bookmarksfly.cn

TS:   nested.flat();
来源：http://hq.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dd.huanxung.cn

Go:   // 手写双层循环
来源：http://sp.nszjky.cn

Ruby: nested.flatten
来源：http://bk.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ge.bookmarksfly.cn

[D19] 按字段分组
来源：http://pz.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vy.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://td.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qt.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ke.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sm.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://tn.hnjuh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sl.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ky.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://hn.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://ul.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://bh.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jr.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tb.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ij.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://on.haigaiapp.cn

Ruby: arr.tally
来源：http://fv.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ey.szsharing.cn

[D21] 判断是否包含某元素
来源：http://vy.jctech888.com.cn

Py:   x in arr
来源：http://ub.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://qx.szxytkj.cn

JS:   arr.includes(x)
来源：http://ov.bjjhwx.cn

TS:   arr.includes(x)
来源：http://ft.huanxung.cn

Java: list.contains(x)
来源：http://db.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://qe.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://tw.521024.cn

C#:   list.Contains(x)
来源：http://kv.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://cc.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://he.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xt.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ve.yuntaijiaju.cn

TS:   [...arr];
来源：http://lx.hahajie.cn

Java: new ArrayList<>(list);
来源：http://vb.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://re.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://mu.hahajie.cn

C#:   new List<int>(list);
来源：http://ds.huixiangedu.cn

[D23] reduce 累积计算
来源：http://zv.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ln.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ba.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dm.shxzskj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gr.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vv.muxihuayi.cn

Go:   // 手写循环
来源：http://tq.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kj.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://np.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://ot.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xh.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sa.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jg.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kd.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://si.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dl.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ki.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yx.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://vz.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tv.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cc.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qu.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cc.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yv.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://us.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ow.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wz.bjjhwx.cn

[D26] 数组转字符串
来源：http://cv.asd995.cn

Py:   ", ".join(map(str, arr))
来源：http://ex.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://oa.nszjky.cn

JS:   arr.join(", ")
来源：http://mc.huixiangedu.cn

TS:   arr.join(", ")
来源：http://sv.panjiajie.cn

Java: String.join(", ", list)
来源：http://eo.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://dg.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://hg.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://fo.wgjwhj.cn

================================================================================
来源：http://gv.szxytkj.cn

E. 字符串处理
来源：http://fc.shxzukj.cn

================================================================================
来源：http://pe.bjjhwx.cn

[E01] 拼接字符串
来源：http://xz.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lk.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fx.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zx.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nr.szxytkj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zs.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ow.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pc.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vr.colortex.cn

[E02] 重复字符串
来源：http://tq.szsharing.cn

Py:   "ab" * 3
来源：http://bp.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://gw.hahajie.cn

JS:   "ab".repeat(3)
来源：http://td.9csxet.cn

TS:   "ab".repeat(3)
来源：http://fu.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://tu.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://th.panjiajie.cn

Ruby: "ab" * 3
来源：http://xf.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ol.bjjhwx.cn

[E03] 截取子串
来源：http://rw.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sk.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pf.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fg.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://ze.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://mh.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://on.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://at.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://sm.szxytkj.cn

[E04] 查找子串位置
来源：http://ty.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://cp.bjjhwx.cn

PHP:  strpos($s, "x");
来源：http://js.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jn.shxzskj.cn

TS:   s.indexOf("x")
来源：http://ws.haigaiapp.cn

Java: s.indexOf("x")
来源：http://ue.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://lw.bookmarksfly.cn

Ruby: s.index("x")
来源：http://op.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://zj.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vo.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ri.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ym.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://re.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qb.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xs.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kf.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iu.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tp.panjiajie.cn

[E06] 替换子串
来源：http://wo.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hw.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://mz.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sj.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://yu.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ax.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://au.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bh.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://hp.huanxung.cn

[E07] 按分隔符拆分
来源：http://tc.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ze.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mo.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cs.shxzukj.cn

TS:   s.split(",")
来源：http://dt.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gb.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kr.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://fu.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pz.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://db.lnxyls.cn

Py:   ",".join(items)
来源：http://ho.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://fi.hahajie.cn

JS:   items.join(",")
来源：http://cb.yuntaijiaju.cn

TS:   items.join(",")
来源：http://rp.newstarts.cn

Java: String.join(",", items)
来源：http://pq.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://cy.huixiangedu.cn

Ruby: items.join(",")
来源：http://gh.9csxet.cn

C#:   string.Join(",", items)
来源：http://yt.colortex.cn

[E09] 去除所有空白字符
来源：http://gb.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gv.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xe.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://al.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://te.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://hy.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lc.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mt.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tk.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://fe.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kl.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ae.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://jm.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://gl.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://bx.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zt.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lf.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hw.jianghongdianzi.cn

[E11] 反转字符串
来源：http://wz.lnxyls.cn

Py:   s[::-1]
来源：http://ah.nicolike.cn

PHP:  strrev($s);
来源：http://sj.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://xs.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://qg.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zl.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yl.lnxyls.cn

Ruby: s.reverse
来源：http://qa.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tv.asd995.cn

[E12] 统计某字符出现次数
来源：http://lb.521024.cn

Py:   s.count("a")
来源：http://br.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://hw.huanxung.cn

JS:   s.split("a").length - 1
来源：http://sw.szsharing.cn

TS:   s.split("a").length - 1
来源：http://ri.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dd.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://ue.nszjky.cn

Ruby: s.count("a")
来源：http://hb.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://yg.colortex.cn

[E13] 逐字符遍历
来源：http://nu.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://bw.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rj.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yl.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ho.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://we.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rv.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://li.haigaiapp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fj.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://vf.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ba.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://py.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vy.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uj.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vu.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vv.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ia.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uh.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://xx.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lt.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cr.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hd.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jl.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ah.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://al.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xo.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vc.gzmigu.cn

[E16] 数字千分位
来源：http://xl.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://xa.9csxet.cn

PHP:  number_format(1234567);
来源：http://af.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xx.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vc.hnjuh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ds.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qw.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xb.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://ds.shxzskj.cn

[E17] 首字母大写
来源：http://dc.nicolike.cn


<!-- 参考信息 -->