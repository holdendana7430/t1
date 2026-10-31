代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mz.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sm.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fz.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qj.hnjuh.cn

[D11] 反转数组
来源：http://tf.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://co.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://cp.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nt.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://xf.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://me.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://hv.szsharing.cn

Ruby: arr.reverse
来源：http://tz.nicolike.cn

C#:   list.Reverse();
来源：http://ty.haigaiapp.cn

[D12] 查找元素下标
来源：http://yl.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://om.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://do.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ig.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tt.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nd.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://zm.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://ry.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://hf.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://lj.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mf.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tj.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://pr.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://xn.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kr.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ij.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lm.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ox.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://ws.bjjhwx.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oa.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mx.521024.cn

JS:   arr.map(x => x * 2)
来源：http://mx.521024.cn

TS:   arr.map(x => x * 2)
来源：http://me.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dq.shxzukj.cn

Go:   // 手写循环
来源：http://aj.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zm.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dn.nszjky.cn

[D15] 去重
来源：http://tj.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lb.gzmigu.cn

PHP:  array_unique($arr);
来源：http://wt.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://tv.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://wg.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pj.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lw.newstarts.cn

Ruby: arr.uniq
来源：http://ak.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://tz.newstarts.cn

[D16] 求和与平均值
来源：http://jx.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://we.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ny.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jo.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ej.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xs.shtwfgs.cn

Go:   // 手写循环累加
来源：http://rj.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ew.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://jr.hnjuh.cn

[D17] 最大值与最小值
来源：http://xs.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://nc.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://qi.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ql.521024.cn

TS:   Math.max(...arr);
来源：http://lr.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hn.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ti.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://rf.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://rw.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://mr.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wf.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://zu.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sx.shxzskj.cn

TS:   nested.flat();
来源：http://kt.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gy.lnxyls.cn

Go:   // 手写双层循环
来源：http://tf.nszjky.cn

Ruby: nested.flatten
来源：http://kv.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ux.yuntaijiaju.cn

[D19] 按字段分组
来源：http://uq.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lk.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gf.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fi.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xv.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dp.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://ke.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ed.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zp.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://up.yuexingan06.cn

Py:   Counter(arr)
来源：http://bb.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://xr.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://md.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dp.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jy.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://hr.huixiangedu.cn

Ruby: arr.tally
来源：http://ip.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bv.colortex.cn

[D21] 判断是否包含某元素
来源：http://gs.huanxung.cn

Py:   x in arr
来源：http://kc.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://iz.hahajie.cn

JS:   arr.includes(x)
来源：http://dm.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://be.shxzukj.cn

Java: list.contains(x)
来源：http://db.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://fn.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://uq.521024.cn

C#:   list.Contains(x)
来源：http://yz.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://pm.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fi.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qs.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ky.newstarts.cn

TS:   [...arr];
来源：http://fn.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://ny.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://db.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://zb.asd995.cn

C#:   new List<int>(list);
来源：http://te.shtwfgs.cn

[D23] reduce 累积计算
来源：http://kj.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fx.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bd.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gq.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dn.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ro.haigaiapp.cn

Go:   // 手写循环
来源：http://xc.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oq.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kq.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://py.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kl.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vg.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://od.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ng.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uc.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gz.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xg.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hh.521024.cn

[D25] Set 集合去重与交并差
来源：http://tj.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ki.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zr.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wc.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dr.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fu.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ew.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vs.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jq.9csxet.cn

[D26] 数组转字符串
来源：http://vx.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://xl.colortex.cn

PHP:  implode(", ", $arr);
来源：http://rf.muxihuayi.cn

JS:   arr.join(", ")
来源：http://in.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://cd.panjiajie.cn

Java: String.join(", ", list)
来源：http://yo.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://hf.huanxung.cn

Ruby: arr.join(", ")
来源：http://bx.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://ca.nicolike.cn

================================================================================
来源：http://jz.jianghongdianzi.cn

E. 字符串处理
来源：http://qs.huixinmuqiang.cn

================================================================================
来源：http://of.jctech888.com.cn

[E01] 拼接字符串
来源：http://dh.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pg.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ne.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://au.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sq.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oi.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sm.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bj.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dv.shtwfgs.cn

[E02] 重复字符串
来源：http://vj.panjiajie.cn

Py:   "ab" * 3
来源：http://np.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://yj.asd995.cn

JS:   "ab".repeat(3)
来源：http://ot.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://fl.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://ku.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://tf.lnxyls.cn

Ruby: "ab" * 3
来源：http://ft.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ys.jianghongdianzi.cn

[E03] 截取子串
来源：http://xo.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jy.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yf.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kw.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://ne.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://nw.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hw.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ux.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://sx.shxzskj.cn

[E04] 查找子串位置
来源：http://lh.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://lu.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://bx.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ej.asd995.cn

TS:   s.indexOf("x")
来源：http://ub.521024.cn

Java: s.indexOf("x")
来源：http://ph.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://nm.szxytkj.cn

Ruby: s.index("x")
来源：http://qz.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://ri.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://es.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xo.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://st.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fc.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://iu.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://di.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nh.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://no.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tp.chemitech.net.cn

[E06] 替换子串
来源：http://vv.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nm.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://ts.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kv.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://ug.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ye.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zf.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ba.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://tl.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://wz.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nb.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ym.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jq.huanxung.cn

TS:   s.split(",")
来源：http://ap.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ds.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ea.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://cj.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cj.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://nu.bookmarksfly.cn

Py:   ",".join(items)
来源：http://io.panjiajie.cn

PHP:  implode(",", $items);
来源：http://ei.bjjhwx.cn

JS:   items.join(",")
来源：http://vz.nszjky.cn

TS:   items.join(",")
来源：http://ip.hahajie.cn

Java: String.join(",", items)
来源：http://rg.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://ip.gzmigu.cn

Ruby: items.join(",")
来源：http://hc.shxzukj.cn

C#:   string.Join(",", items)
来源：http://fc.9csxet.cn

[E09] 去除所有空白字符
来源：http://mc.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rc.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yk.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://am.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://vr.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://za.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tx.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dp.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ws.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://jw.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oi.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bo.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://ao.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://ad.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://xc.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ce.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wu.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qi.yuntaijiaju.cn

[E11] 反转字符串
来源：http://aa.nicolike.cn

Py:   s[::-1]
来源：http://lv.szsharing.cn

PHP:  strrev($s);
来源：http://iu.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://vl.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://nf.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pn.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kt.muxihuayi.cn

Ruby: s.reverse
来源：http://bf.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ku.shtwfgs.cn

[E12] 统计某字符出现次数
来源：http://fl.nszjky.cn

Py:   s.count("a")
来源：http://jb.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://te.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://ye.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://wm.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lz.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://kq.shtwfgs.cn

Ruby: s.count("a")
来源：http://yv.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://wl.lnxyls.cn

[E13] 逐字符遍历
来源：http://gm.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://ej.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oo.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kh.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://or.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gr.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vx.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xu.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ry.shxzskj.cn

[E14] URL 编码与 Base64
来源：http://ml.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ir.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ns.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hc.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hh.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ax.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dm.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lp.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://id.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://mi.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uy.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ri.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fa.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fq.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nk.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yt.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://og.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hv.shxzukj.cn

[E16] 数字千分位
来源：http://ta.hahajie.cn

Py:   f"{1234567:,}"
来源：http://ye.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://ti.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bs.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gp.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ab.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dc.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tj.asd995.cn

C#:   1234567.ToString("N0")
来源：http://il.521024.cn

[E17] 首字母大写
来源：http://ht.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ef.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ez.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jv.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sy.wgjwhj.cn


<!-- 参考信息 -->