代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ep.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://zw.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://hq.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gk.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ng.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bh.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hb.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://bf.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gv.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rm.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://kk.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://pv.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://an.colortex.cn

Go:   // 手写循环
来源：http://yw.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vz.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jg.haigaiapp.cn

[D15] 去重
来源：http://de.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gk.colortex.cn

PHP:  array_unique($arr);
来源：http://ls.hahajie.cn

JS:   [...new Set(arr)]
来源：http://aw.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://st.huixiangedu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kn.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vk.szsharing.cn

Ruby: arr.uniq
来源：http://tv.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://tn.shtwfgs.cn

[D16] 求和与平均值
来源：http://oa.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ew.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gu.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ax.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nt.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uj.huanxung.cn

Go:   // 手写循环累加
来源：http://fm.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uj.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://zy.wgjwhj.cn

[D17] 最大值与最小值
来源：http://qj.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://wg.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://xp.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://me.nszjky.cn

TS:   Math.max(...arr);
来源：http://nh.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nc.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nh.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://ic.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://sa.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://ff.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rq.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://ax.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mp.szxytkj.cn

TS:   nested.flat();
来源：http://rn.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://te.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://gx.hahajie.cn

Ruby: nested.flatten
来源：http://bj.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://il.panjiajie.cn

[D19] 按字段分组
来源：http://ow.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xw.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pe.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nd.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vc.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vy.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://tn.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://md.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uf.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://ms.shxzukj.cn

Py:   Counter(arr)
来源：http://wo.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://hc.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yi.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ne.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vz.newstarts.cn

Go:   // 手写 map[T]int
来源：http://hd.bjjhwx.cn

Ruby: arr.tally
来源：http://cs.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pn.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://za.panjiajie.cn

Py:   x in arr
来源：http://kl.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://py.jctech888.com.cn

JS:   arr.includes(x)
来源：http://lh.shxzskj.cn

TS:   arr.includes(x)
来源：http://og.panjiajie.cn

Java: list.contains(x)
来源：http://gs.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://zd.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://hn.haigaiapp.cn

C#:   list.Contains(x)
来源：http://yq.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://mb.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://um.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zn.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hj.szxytkj.cn

TS:   [...arr];
来源：http://gx.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://tg.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hf.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://uu.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://qh.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://qo.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mq.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bo.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nu.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qn.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://py.lnxyls.cn

Go:   // 手写循环
来源：http://py.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://st.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nm.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://yv.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uv.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mn.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hi.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yc.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ma.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xl.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ff.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://eq.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://wa.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tu.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hp.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ku.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dt.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hp.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ky.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xw.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zx.shtwfgs.cn

[D26] 数组转字符串
来源：http://kg.asd995.cn

Py:   ", ".join(map(str, arr))
来源：http://oz.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://hp.hnjuh.cn

JS:   arr.join(", ")
来源：http://hx.wgjwhj.cn

TS:   arr.join(", ")
来源：http://vt.chemitech.net.cn

Java: String.join(", ", list)
来源：http://dp.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://qv.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://kn.nicolike.cn

C#:   string.Join(", ", list)
来源：http://ul.newstarts.cn

================================================================================
来源：http://vh.gzmigu.cn

E. 字符串处理
来源：http://gd.panjiajie.cn

================================================================================
来源：http://rd.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://lb.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hn.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pw.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nu.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gi.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jm.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nl.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://io.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qm.shxzukj.cn

[E02] 重复字符串
来源：http://zd.gzmigu.cn

Py:   "ab" * 3
来源：http://hr.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://il.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://pq.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://tp.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://ox.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://rc.shxzukj.cn

Ruby: "ab" * 3
来源：http://aj.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://at.nicolike.cn

[E03] 截取子串
来源：http://oh.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ry.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qo.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://el.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://co.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://ii.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zo.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://se.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://ul.haigaiapp.cn

[E04] 查找子串位置
来源：http://je.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://ol.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://ek.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qa.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://yg.jctech888.com.cn

Java: s.indexOf("x")
来源：http://ku.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://ym.muxihuayi.cn

Ruby: s.index("x")
来源：http://ce.huanxung.cn

C#:   s.IndexOf("x")
来源：http://xv.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lf.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ex.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ri.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oc.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://up.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gq.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ti.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qi.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tx.panjiajie.cn

[E06] 替换子串
来源：http://eu.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vb.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://st.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dx.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://tp.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bs.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rg.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ka.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://db.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://vn.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qu.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vg.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ff.chemitech.net.cn

TS:   s.split(",")
来源：http://ou.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bo.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zk.colortex.cn

Ruby: s.split(",");  s.split
来源：http://sd.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sb.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://is.hahajie.cn

Py:   ",".join(items)
来源：http://zb.shxzskj.cn

PHP:  implode(",", $items);
来源：http://nw.yuexingan06.cn

JS:   items.join(",")
来源：http://fn.9csxet.cn

TS:   items.join(",")
来源：http://ov.muxihuayi.cn

Java: String.join(",", items)
来源：http://nf.colortex.cn

Go:   strings.Join(items, ",")
来源：http://dw.huixiangedu.cn

Ruby: items.join(",")
来源：http://iq.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://yj.nszjky.cn

[E09] 去除所有空白字符
来源：http://cr.shxzskj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ry.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pn.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://rx.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://rk.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://gl.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://by.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cq.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hh.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://aq.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kw.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sz.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://ij.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://rw.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://rx.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uh.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xg.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yb.yuexingan06.cn

[E11] 反转字符串
来源：http://fo.huixiangedu.cn

Py:   s[::-1]
来源：http://lt.nicolike.cn

PHP:  strrev($s);
来源：http://dz.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://ha.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://tv.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dc.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uj.9csxet.cn

Ruby: s.reverse
来源：http://no.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wy.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://vs.nszjky.cn

Py:   s.count("a")
来源：http://hy.szxytkj.cn

PHP:  substr_count($s, "a");
来源：http://zf.huanxung.cn

JS:   s.split("a").length - 1
来源：http://yd.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://ql.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pg.521024.cn

Go:   strings.Count(s, "a")
来源：http://qi.shxzskj.cn

Ruby: s.count("a")
来源：http://wj.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://rz.lnxyls.cn

[E13] 逐字符遍历
来源：http://pe.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://tn.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ll.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ry.asd995.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ri.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zl.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qb.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bx.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jr.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://sq.hahajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uc.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qc.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nm.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://io.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ui.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://do.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xe.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sr.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://hp.colortex.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gx.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bk.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gc.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dr.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://af.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qe.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rv.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ie.muxihuayi.cn

[E16] 数字千分位
来源：http://ed.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://ms.nszjky.cn

PHP:  number_format(1234567);
来源：http://pb.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yz.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ds.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nj.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ps.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://en.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://pl.gzmigu.cn

[E17] 首字母大写
来源：http://co.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wi.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gs.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zc.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cw.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ir.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ls.hnjuh.cn

Ruby: s.capitalize
来源：http://fr.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sb.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://vu.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ur.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://md.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://oo.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://os.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ui.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ga.newstarts.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wv.nszjky.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ph.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://fd.colortex.cn

Py:   s.splitlines()
来源：http://hs.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vh.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://dy.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://eo.szsharing.cn

Java: s.lines().toList()
来源：http://td.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://vr.gzmigu.cn

Ruby: s.lines
来源：http://aj.huanxung.cn

C#:   s.Split('\n')
来源：http://fi.nicolike.cn

[E20] 判断字符串是否为空
来源：http://yt.asd995.cn

Py:   if not s:
来源：http://ag.lnxyls.cn


<!-- 参考信息 -->