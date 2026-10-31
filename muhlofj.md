代发 wailian999

[D15] 去重
来源：http://wa.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yk.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://bv.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://uj.hahajie.cn

TS:   [...new Set(arr)]
来源：http://of.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qs.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rz.521024.cn

Ruby: arr.uniq
来源：http://dr.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://qm.shxzukj.cn

[D16] 求和与平均值
来源：http://md.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ui.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wv.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hb.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wd.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jq.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://da.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mj.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://kp.haigaiapp.cn

[D17] 最大值与最小值
来源：http://gv.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://wx.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://kf.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wn.shxzukj.cn

TS:   Math.max(...arr);
来源：http://gn.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kb.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iw.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://ay.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://yt.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://vr.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jh.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://wx.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ei.hahajie.cn

TS:   nested.flat();
来源：http://ul.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bh.panjiajie.cn

Go:   // 手写双层循环
来源：http://sd.asd995.cn

Ruby: nested.flatten
来源：http://zb.wgjwhj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ne.wgjwhj.cn

[D19] 按字段分组
来源：http://oi.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ed.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lx.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wd.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://un.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qa.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://ca.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ym.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oh.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://xe.szxytkj.cn

Py:   Counter(arr)
来源：http://qo.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://ns.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bh.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cv.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bw.colortex.cn

Go:   // 手写 map[T]int
来源：http://py.hahajie.cn

Ruby: arr.tally
来源：http://sp.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qp.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://lv.huixinmuqiang.cn

Py:   x in arr
来源：http://jw.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://db.huixiangedu.cn

JS:   arr.includes(x)
来源：http://lh.panjiajie.cn

TS:   arr.includes(x)
来源：http://kk.lnxyls.cn

Java: list.contains(x)
来源：http://pw.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://wq.szxytkj.cn

Ruby: arr.include?(x)
来源：http://yz.gzmigu.cn

C#:   list.Contains(x)
来源：http://dl.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://gv.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jd.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://at.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xo.521024.cn

TS:   [...arr];
来源：http://xc.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://ji.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uy.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://er.shxzukj.cn

C#:   new List<int>(list);
来源：http://te.huanxung.cn

[D23] reduce 累积计算
来源：http://vp.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ll.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://is.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qd.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mn.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ce.szxytkj.cn

Go:   // 手写循环
来源：http://pk.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ln.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dj.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://bv.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://as.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sm.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vu.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ye.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iv.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iw.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://am.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://my.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://uc.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eb.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ir.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://se.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ay.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kg.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oe.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sh.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rx.nicolike.cn

[D26] 数组转字符串
来源：http://gv.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://ij.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://go.huanxung.cn

JS:   arr.join(", ")
来源：http://jb.asd995.cn

TS:   arr.join(", ")
来源：http://os.colortex.cn

Java: String.join(", ", list)
来源：http://bk.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://pb.shxzukj.cn

Ruby: arr.join(", ")
来源：http://lp.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://rk.jctech888.com.cn

================================================================================
来源：http://iy.szxytkj.cn

E. 字符串处理
来源：http://kw.hnjuh.cn

================================================================================
来源：http://ea.shxzukj.cn

[E01] 拼接字符串
来源：http://xx.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ao.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ts.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ae.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eu.yuntaijiaju.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dh.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bo.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pa.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fh.hahajie.cn

[E02] 重复字符串
来源：http://qn.wgjwhj.cn

Py:   "ab" * 3
来源：http://rf.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://bp.newstarts.cn

JS:   "ab".repeat(3)
来源：http://qf.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://io.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://yf.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://fr.shtwfgs.cn

Ruby: "ab" * 3
来源：http://ns.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lc.chemitech.net.cn

[E03] 截取子串
来源：http://aw.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bu.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wz.gzmigu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gv.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://su.lnxyls.cn

Java: s.substring(1, 4)
来源：http://nw.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qc.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wk.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://wt.chemitech.net.cn

[E04] 查找子串位置
来源：http://dd.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://zg.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://nk.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hd.shxzukj.cn

TS:   s.indexOf("x")
来源：http://kj.9csxet.cn

Java: s.indexOf("x")
来源：http://hv.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://es.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://jv.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://fg.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://od.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kx.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nx.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tb.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://us.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://px.nicolike.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kz.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ix.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ow.panjiajie.cn

[E06] 替换子串
来源：http://tm.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://su.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://gk.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gb.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://gw.asd995.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xq.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tl.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yr.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://vl.szxytkj.cn

[E07] 按分隔符拆分
来源：http://kk.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kt.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pj.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rd.bookmarksfly.cn

TS:   s.split(",")
来源：http://gl.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wr.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pt.521024.cn

Ruby: s.split(",");  s.split
来源：http://kq.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sk.nszjky.cn

[E08] 数组按分隔符合并
来源：http://bz.hnjuh.cn

Py:   ",".join(items)
来源：http://qq.asd995.cn

PHP:  implode(",", $items);
来源：http://ds.bookmarksfly.cn

JS:   items.join(",")
来源：http://nc.chemitech.net.cn

TS:   items.join(",")
来源：http://yr.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://zg.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://zx.szxytkj.cn

Ruby: items.join(",")
来源：http://zh.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://dy.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://ho.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://it.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xp.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://oy.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://kj.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://jy.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pk.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qw.wgjwhj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://po.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://ue.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gs.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xy.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://rl.lnxyls.cn

TS:   "7".padStart(3, "0")
来源：http://lp.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://nu.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ib.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kg.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bq.shxzukj.cn

[E11] 反转字符串
来源：http://tx.jctech888.com.cn

Py:   s[::-1]
来源：http://mi.nicolike.cn

PHP:  strrev($s);
来源：http://tm.colortex.cn

JS:   [...s].reverse().join("")
来源：http://ly.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://qo.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ke.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://em.bookmarksfly.cn

Ruby: s.reverse
来源：http://wm.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qj.bjjhwx.cn

[E12] 统计某字符出现次数
来源：http://st.hnjuh.cn

Py:   s.count("a")
来源：http://le.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://jr.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://lg.521024.cn

TS:   s.split("a").length - 1
来源：http://ti.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ab.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://eu.bjjhwx.cn

Ruby: s.count("a")
来源：http://rq.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://ze.szsharing.cn

[E13] 逐字符遍历
来源：http://vl.colortex.cn

Py:   for ch in s: print(ch)
来源：http://nk.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ho.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vv.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://aq.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gw.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ms.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nu.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lh.shxzskj.cn

[E14] URL 编码与 Base64
来源：http://vh.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bz.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://so.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tc.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bl.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mx.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ab.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qb.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pr.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://ce.bjjhwx.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bu.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ed.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ea.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sp.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sz.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gq.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://us.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gl.9csxet.cn

[E16] 数字千分位
来源：http://jq.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://fg.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://ad.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nz.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wv.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qs.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://je.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pm.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://ti.nicolike.cn

[E17] 首字母大写
来源：http://tm.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://un.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sx.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ph.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dy.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://am.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gx.panjiajie.cn

Ruby: s.capitalize
来源：http://ck.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hw.shxzukj.cn

[E18] 模板占位符替换
来源：http://ga.chemitech.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nd.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cr.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tx.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ri.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kw.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://am.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mz.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qh.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://lr.jctech888.com.cn

Py:   s.splitlines()
来源：http://iu.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qo.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://wv.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://vb.colortex.cn

Java: s.lines().toList()
来源：http://yk.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://hf.yuexingan06.cn

Ruby: s.lines
来源：http://we.521024.cn

C#:   s.Split('\n')
来源：http://qn.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://kv.shxzskj.cn

Py:   if not s:
来源：http://qc.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oz.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://le.yuexingan06.cn

TS:   if (s === "") {}
来源：http://fx.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://ju.szxytkj.cn

Go:   if s == "" {}
来源：http://mz.bookmarksfly.cn

Ruby: if s.empty?
来源：http://rn.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xs.shxzukj.cn

[E21] 超长截断加省略号
来源：http://on.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iv.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bh.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wu.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qj.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gk.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://un.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oi.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vy.shtwfgs.cn


<!-- 参考信息 -->