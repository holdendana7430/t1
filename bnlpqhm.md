代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xu.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pz.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kd.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bk.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://br.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pw.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ny.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gn.shxzskj.cn

[D11] 反转数组
来源：http://dz.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sf.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://ww.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vp.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://tx.shxzskj.cn

Java: Collections.reverse(list);
来源：http://yt.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://xl.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://uf.szsharing.cn

C#:   list.Reverse();
来源：http://qz.muxihuayi.cn

[D12] 查找元素下标
来源：http://uj.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://ju.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tg.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ds.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yo.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ut.asd995.cn

Go:   slices.Index(arr, x)
来源：http://sd.yuexingan06.cn

Ruby: arr.index(x)
来源：http://rg.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://wt.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://on.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fe.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jl.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://zw.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://st.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dq.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ay.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://es.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://si.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://gv.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tv.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mc.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://at.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://cr.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wo.asd995.cn

Go:   // 手写循环
来源：http://sr.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xz.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xf.521024.cn

[D15] 去重
来源：http://vf.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zy.huanxung.cn

PHP:  array_unique($arr);
来源：http://wz.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://oj.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://ih.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fd.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uz.panjiajie.cn

Ruby: arr.uniq
来源：http://it.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://wy.bjjhwx.cn

[D16] 求和与平均值
来源：http://rs.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hd.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nx.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jm.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cm.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wf.huixiangedu.cn

Go:   // 手写循环累加
来源：http://lc.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ya.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://sj.hahajie.cn

[D17] 最大值与最小值
来源：http://vg.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://un.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://ng.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ul.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://bl.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ec.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gq.huixinmuqiang.cn

Ruby: arr.max;  arr.min
来源：http://kf.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://cp.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://lx.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ty.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://bx.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yl.bjjhwx.cn

TS:   nested.flat();
来源：http://nb.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pi.asd995.cn

Go:   // 手写双层循环
来源：http://ox.colortex.cn

Ruby: nested.flatten
来源：http://vh.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yg.huanxung.cn

[D19] 按字段分组
来源：http://rt.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bl.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ec.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sg.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rl.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ah.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://jg.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://aq.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oy.colortex.cn

[D20] 统计每个元素出现次数
来源：http://zl.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://ot.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://tk.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://da.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://do.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xw.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://ry.nszjky.cn

Ruby: arr.tally
来源：http://ad.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dl.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://zj.521024.cn

Py:   x in arr
来源：http://ch.shtwfgs.cn

PHP:  in_array($x, $arr, true);
来源：http://ws.yuntaijiaju.cn

JS:   arr.includes(x)
来源：http://df.huixiangedu.cn

TS:   arr.includes(x)
来源：http://ce.lnxyls.cn

Java: list.contains(x)
来源：http://gz.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://yv.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://yz.muxihuayi.cn

C#:   list.Contains(x)
来源：http://vm.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://uw.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ut.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://to.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kd.huixiangedu.cn

TS:   [...arr];
来源：http://gs.newstarts.cn

Java: new ArrayList<>(list);
来源：http://ix.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://be.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://py.szsharing.cn

C#:   new List<int>(list);
来源：http://su.yuexingan06.cn

[D23] reduce 累积计算
来源：http://eq.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dq.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sh.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dq.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://um.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xs.shxzukj.cn

Go:   // 手写循环
来源：http://eo.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zf.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aw.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://we.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rh.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bx.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bt.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jo.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yg.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gk.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ec.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qs.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://yr.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ub.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zm.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pf.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xz.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vn.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ek.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pj.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ym.521024.cn

[D26] 数组转字符串
来源：http://dr.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://ll.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://ob.wgjwhj.cn

JS:   arr.join(", ")
来源：http://iv.huixiangedu.cn

TS:   arr.join(", ")
来源：http://qu.nszjky.cn

Java: String.join(", ", list)
来源：http://zy.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://by.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://ta.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://sk.lnxyls.cn

================================================================================
来源：http://yz.jctech888.com.cn

E. 字符串处理
来源：http://uk.nicolike.cn

================================================================================
来源：http://uz.huanxung.cn

[E01] 拼接字符串
来源：http://dl.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wy.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://aw.szsharing.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gm.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gv.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fu.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gl.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wp.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wq.shxzukj.cn

[E02] 重复字符串
来源：http://xt.haigaiapp.cn

Py:   "ab" * 3
来源：http://ok.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://id.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://io.newstarts.cn

TS:   "ab".repeat(3)
来源：http://jq.szsharing.cn

Java: "ab".repeat(3)
来源：http://vr.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://rf.jctech888.com.cn

Ruby: "ab" * 3
来源：http://ks.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://at.jianghongdianzi.cn

[E03] 截取子串
来源：http://or.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qn.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pq.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cv.521024.cn

TS:   s.slice(1, 4)
来源：http://az.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://qi.shtwfgs.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ki.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://eg.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://oa.wgjwhj.cn

[E04] 查找子串位置
来源：http://ny.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://hd.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://mw.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ky.hahajie.cn

TS:   s.indexOf("x")
来源：http://jr.szxytkj.cn

Java: s.indexOf("x")
来源：http://kb.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://tx.bjjhwx.cn

Ruby: s.index("x")
来源：http://cc.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://ip.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fu.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kc.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mc.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://is.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nm.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vo.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fr.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pf.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ga.bjjhwx.cn

[E06] 替换子串
来源：http://bo.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rm.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://au.nszjky.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sf.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://mx.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rj.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://po.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rk.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://sz.shxzskj.cn

[E07] 按分隔符拆分
来源：http://yv.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zv.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vg.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mk.huixiangedu.cn

TS:   s.split(",")
来源：http://uv.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ol.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iy.colortex.cn

Ruby: s.split(",");  s.split
来源：http://sz.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://om.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://wb.huixiangedu.cn

Py:   ",".join(items)
来源：http://uc.huanxung.cn

PHP:  implode(",", $items);
来源：http://lf.szsharing.cn

JS:   items.join(",")
来源：http://fb.jctech888.com.cn

TS:   items.join(",")
来源：http://ln.9csxet.cn

Java: String.join(",", items)
来源：http://zi.521024.cn

Go:   strings.Join(items, ",")
来源：http://sn.jctech888.com.cn

Ruby: items.join(",")
来源：http://kg.nszjky.cn

C#:   string.Join(",", items)
来源：http://cx.hnjuh.cn

[E09] 去除所有空白字符
来源：http://jl.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bb.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://us.bookmarksfly.cn

JS:   s.replace(/\s+/g, "")
来源：http://rm.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://bp.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://tw.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ge.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gz.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lx.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://ig.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hc.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nu.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://li.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://sd.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://cy.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ap.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pw.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kn.gzmigu.cn

[E11] 反转字符串
来源：http://yv.yuntaijiaju.cn

Py:   s[::-1]
来源：http://kz.bookmarksfly.cn

PHP:  strrev($s);
来源：http://ln.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://tg.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://mj.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dv.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pk.gzmigu.cn

Ruby: s.reverse
来源：http://xl.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ft.nicolike.cn

[E12] 统计某字符出现次数
来源：http://pl.yuntaijiaju.cn

Py:   s.count("a")
来源：http://zt.asd995.cn

PHP:  substr_count($s, "a");
来源：http://wr.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://jj.nicolike.cn

TS:   s.split("a").length - 1
来源：http://kk.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ny.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://rf.bookmarksfly.cn

Ruby: s.count("a")
来源：http://ar.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://tl.hnjuh.cn

[E13] 逐字符遍历
来源：http://bs.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://qs.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ln.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sr.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mm.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gn.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kp.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://il.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tm.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://lw.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xu.gzmigu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tw.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pw.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://js.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kj.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sx.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://up.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xb.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://mc.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xs.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fs.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ri.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://uk.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qi.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tv.hahajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://od.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ol.yuexingan06.cn

[E16] 数字千分位
来源：http://kc.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://da.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://wy.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yk.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xm.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vt.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xa.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vo.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://xt.szxytkj.cn

[E17] 首字母大写
来源：http://qg.newstarts.cn


<!-- 参考信息 -->