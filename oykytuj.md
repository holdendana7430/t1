代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ij.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gk.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xw.newstarts.cn

[D14] 映射转换（每个元素变形）
来源：http://hi.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dx.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://in.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://dn.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://zv.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gn.bjjhwx.cn

Go:   // 手写循环
来源：http://bd.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lf.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yh.szxytkj.cn

[D15] 去重
来源：http://ev.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dt.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://xo.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://su.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://ny.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rp.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jh.szxytkj.cn

Ruby: arr.uniq
来源：http://za.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://kz.szxytkj.cn

[D16] 求和与平均值
来源：http://uw.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ic.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sv.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://er.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iw.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qk.haigaiapp.cn

Go:   // 手写循环累加
来源：http://uy.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sf.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://ul.huanxung.cn

[D17] 最大值与最小值
来源：http://kb.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://kc.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://sg.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vh.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://rx.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zb.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ey.asd995.cn

Ruby: arr.max;  arr.min
来源：http://bo.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://rp.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://qd.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ij.asd995.cn

PHP:  array_merge(...$nested);
来源：http://ut.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qz.szxytkj.cn

TS:   nested.flat();
来源：http://kp.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ua.hahajie.cn

Go:   // 手写双层循环
来源：http://zn.huanxung.cn

Ruby: nested.flatten
来源：http://sz.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cm.gzmigu.cn

[D19] 按字段分组
来源：http://tj.nicolike.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mc.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rp.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ed.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kt.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qb.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://ez.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mc.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jw.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://cr.hnjuh.cn

Py:   Counter(arr)
来源：http://uk.9csxet.cn

PHP:  array_count_values($arr);
来源：http://za.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ru.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kn.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dh.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://gt.bookmarksfly.cn

Ruby: arr.tally
来源：http://nr.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sq.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://gp.shxzskj.cn

Py:   x in arr
来源：http://ld.shtwfgs.cn

PHP:  in_array($x, $arr, true);
来源：http://pm.haigaiapp.cn

JS:   arr.includes(x)
来源：http://cy.panjiajie.cn

TS:   arr.includes(x)
来源：http://zi.gzmigu.cn

Java: list.contains(x)
来源：http://fk.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://lm.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://bd.521024.cn

C#:   list.Contains(x)
来源：http://tw.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://lz.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yk.hnjuh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bp.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rf.hnjuh.cn

TS:   [...arr];
来源：http://oc.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://kh.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://da.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://ga.nicolike.cn

C#:   new List<int>(list);
来源：http://po.muxihuayi.cn

[D23] reduce 累积计算
来源：http://hv.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mb.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iq.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ff.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gs.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ia.bookmarksfly.cn

Go:   // 手写循环
来源：http://bl.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gm.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sp.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://di.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hv.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wy.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dj.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ip.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ta.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wi.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sl.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://le.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://qv.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mn.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bz.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tm.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oc.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ap.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ag.wgjwhj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hx.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.nicolike.cn

[D26] 数组转字符串
来源：http://kw.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://jp.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://pp.nicolike.cn

JS:   arr.join(", ")
来源：http://ou.shtwfgs.cn

TS:   arr.join(", ")
来源：http://vr.szsharing.cn

Java: String.join(", ", list)
来源：http://pr.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://zw.hahajie.cn

Ruby: arr.join(", ")
来源：http://mf.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://xt.szxytkj.cn

================================================================================
来源：http://qa.bookmarksfly.cn

E. 字符串处理
来源：http://fd.bookmarksfly.cn

================================================================================
来源：http://da.shxzskj.cn

[E01] 拼接字符串
来源：http://lv.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eu.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ej.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ml.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sn.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ix.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pj.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://om.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fr.szsharing.cn

[E02] 重复字符串
来源：http://wv.521024.cn

Py:   "ab" * 3
来源：http://wr.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://jw.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://bi.asd995.cn

TS:   "ab".repeat(3)
来源：http://so.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://gv.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://ku.muxihuayi.cn

Ruby: "ab" * 3
来源：http://kn.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zj.bjjhwx.cn

[E03] 截取子串
来源：http://gt.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fe.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fo.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sg.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://yn.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://dw.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ok.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://am.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://qv.asd995.cn

[E04] 查找子串位置
来源：http://ea.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://rv.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://fc.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hk.9csxet.cn

TS:   s.indexOf("x")
来源：http://rq.yuexingan06.cn

Java: s.indexOf("x")
来源：http://ew.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://eu.shtwfgs.cn

Ruby: s.index("x")
来源：http://qs.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://nq.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://un.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kn.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ii.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cv.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://su.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uf.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tg.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zd.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kc.hnjuh.cn

[E06] 替换子串
来源：http://rc.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ic.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://ni.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oo.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://io.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dv.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pm.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vw.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://if.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://ix.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ap.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yl.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jh.nicolike.cn

TS:   s.split(",")
来源：http://ww.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kx.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://st.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://jg.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iw.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://ja.szsharing.cn

Py:   ",".join(items)
来源：http://jc.colortex.cn

PHP:  implode(",", $items);
来源：http://xb.newstarts.cn

JS:   items.join(",")
来源：http://we.huixiangedu.cn

TS:   items.join(",")
来源：http://zp.shtwfgs.cn

Java: String.join(",", items)
来源：http://ex.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://iw.asd995.cn

Ruby: items.join(",")
来源：http://hk.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://re.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://bi.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nj.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zt.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://jn.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://ex.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://zz.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vh.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xy.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://db.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://nv.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jg.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fv.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://ml.lnxyls.cn

TS:   "7".padStart(3, "0")
来源：http://ly.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://ea.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uw.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ae.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qw.asd995.cn

[E11] 反转字符串
来源：http://pd.colortex.cn

Py:   s[::-1]
来源：http://wu.nszjky.cn

PHP:  strrev($s);
来源：http://nz.521024.cn

JS:   [...s].reverse().join("")
来源：http://vh.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://iw.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cs.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://um.colortex.cn

Ruby: s.reverse
来源：http://uv.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ku.521024.cn

[E12] 统计某字符出现次数
来源：http://tk.muxihuayi.cn

Py:   s.count("a")
来源：http://bm.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://vz.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://qa.yuexingan06.cn

TS:   s.split("a").length - 1
来源：http://bn.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vk.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://se.newstarts.cn

Ruby: s.count("a")
来源：http://gt.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://nn.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://ij.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://gw.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sj.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xg.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zk.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dn.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sd.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xw.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://db.9csxet.cn

[E14] URL 编码与 Base64
来源：http://aq.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gu.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fv.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://di.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lb.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mo.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yd.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jd.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kz.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://ir.bjjhwx.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vk.haigaiapp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://az.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bh.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ou.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pe.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tc.huixinmuqiang.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://el.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ei.gzmigu.cn

[E16] 数字千分位
来源：http://yy.hahajie.cn

Py:   f"{1234567:,}"
来源：http://ah.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://bv.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hh.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://iw.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bo.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cm.colortex.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yp.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://cu.colortex.cn

[E17] 首字母大写
来源：http://pw.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://un.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://oq.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fp.yuntaijiaju.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uc.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ed.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ry.9csxet.cn

Ruby: s.capitalize
来源：http://pc.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://do.jctech888.com.cn

[E18] 模板占位符替换
来源：http://wq.chemitech.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://va.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qn.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xz.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jt.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nb.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://al.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xv.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rn.nszjky.cn

[E19] 多行文本按行拆分
来源：http://jm.chemitech.net.cn

Py:   s.splitlines()
来源：http://xc.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ik.521024.cn

JS:   s.split(/\r?\n/)
来源：http://ds.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://aq.muxihuayi.cn

Java: s.lines().toList()
来源：http://dr.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://vv.chemitech.net.cn

Ruby: s.lines
来源：http://tu.yuexingan06.cn

C#:   s.Split('\n')
来源：http://zx.nszjky.cn

[E20] 判断字符串是否为空
来源：http://ll.yuntaijiaju.cn

Py:   if not s:
来源：http://ds.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wd.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rn.hahajie.cn

TS:   if (s === "") {}
来源：http://yh.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://hm.muxihuayi.cn


<!-- 参考信息 -->