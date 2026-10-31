代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mk.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://aq.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://kr.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://ql.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://qv.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mi.bookmarksfly.cn

TS:   Math.max(...arr);
来源：http://re.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mn.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zu.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://au.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://xi.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://tu.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zd.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://yz.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tv.lnxyls.cn

TS:   nested.flat();
来源：http://ok.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ch.newstarts.cn

Go:   // 手写双层循环
来源：http://sq.nicolike.cn

Ruby: nested.flatten
来源：http://lk.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://eb.asd995.cn

[D19] 按字段分组
来源：http://bv.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ii.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://av.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bc.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lw.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ka.jianghongdianzi.cn

Go:   // 手写 map[string][]T
来源：http://ak.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://id.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fv.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://hv.9csxet.cn

Py:   Counter(arr)
来源：http://oj.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://vu.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mf.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qi.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vj.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://md.yuexingan06.cn

Ruby: arr.tally
来源：http://hx.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://za.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://ww.hnjuh.cn

Py:   x in arr
来源：http://om.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://ff.szsharing.cn

JS:   arr.includes(x)
来源：http://vk.szsharing.cn

TS:   arr.includes(x)
来源：http://vh.muxihuayi.cn

Java: list.contains(x)
来源：http://ey.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://jk.shxzskj.cn

Ruby: arr.include?(x)
来源：http://dt.hahajie.cn

C#:   list.Contains(x)
来源：http://kz.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://ng.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pq.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hj.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sr.jctech888.com.cn

TS:   [...arr];
来源：http://op.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://oa.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xc.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://gi.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://an.shxzukj.cn

[D23] reduce 累积计算
来源：http://dl.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jg.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ki.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sf.muxihuayi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yk.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oo.szsharing.cn

Go:   // 手写循环
来源：http://bo.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xa.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nn.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://tc.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bq.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sv.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fg.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sr.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nd.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oh.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dq.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uv.colortex.cn

[D25] Set 集合去重与交并差
来源：http://cs.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ks.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xd.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://np.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ag.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fs.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hd.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mi.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wc.muxihuayi.cn

[D26] 数组转字符串
来源：http://wa.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://yv.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://ot.muxihuayi.cn

JS:   arr.join(", ")
来源：http://bb.gzmigu.cn

TS:   arr.join(", ")
来源：http://go.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://mk.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://wx.szxytkj.cn

Ruby: arr.join(", ")
来源：http://gu.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://uw.huixinmuqiang.cn

================================================================================
来源：http://as.szsharing.cn

E. 字符串处理
来源：http://uk.lnxyls.cn

================================================================================
来源：http://ze.521024.cn

[E01] 拼接字符串
来源：http://oi.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vr.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gn.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lo.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ue.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ef.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ii.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tu.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vv.szxytkj.cn

[E02] 重复字符串
来源：http://pd.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://ei.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://rt.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://il.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://fu.huanxung.cn

Java: "ab".repeat(3)
来源：http://ku.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://xs.szxytkj.cn

Ruby: "ab" * 3
来源：http://ll.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xw.szsharing.cn

[E03] 截取子串
来源：http://zf.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ni.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://js.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jy.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://vk.jctech888.com.cn

Java: s.substring(1, 4)
来源：http://ef.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tq.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ey.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://ua.hnjuh.cn

[E04] 查找子串位置
来源：http://cu.asd995.cn

Py:   s.find("x");  s.index("x")
来源：http://rx.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://em.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://er.asd995.cn

TS:   s.indexOf("x")
来源：http://mc.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://bv.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://sb.gzmigu.cn

Ruby: s.index("x")
来源：http://dl.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://cr.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bm.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hd.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dh.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://et.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bx.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nw.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yp.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rs.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wq.szxytkj.cn

[E06] 替换子串
来源：http://ku.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ba.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://vw.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ao.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://hr.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xh.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ca.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yk.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://zx.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://bv.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sp.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qa.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sh.bjjhwx.cn

TS:   s.split(",")
来源：http://au.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ic.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ff.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://fn.jianghongdianzi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fy.nszjky.cn

[E08] 数组按分隔符合并
来源：http://nj.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://td.nszjky.cn

PHP:  implode(",", $items);
来源：http://vh.nicolike.cn

JS:   items.join(",")
来源：http://oy.521024.cn

TS:   items.join(",")
来源：http://vl.huanxung.cn

Java: String.join(",", items)
来源：http://mr.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://io.hnjuh.cn

Ruby: items.join(",")
来源：http://fi.szxytkj.cn

C#:   string.Join(",", items)
来源：http://mv.hahajie.cn

[E09] 去除所有空白字符
来源：http://so.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zb.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ab.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://nl.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://kz.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://ia.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zo.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://aw.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xe.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://gv.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qy.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yt.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://yz.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://rk.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://xz.wgjwhj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hf.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qc.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ao.bookmarksfly.cn

[E11] 反转字符串
来源：http://wu.bjjhwx.cn

Py:   s[::-1]
来源：http://vf.szsharing.cn

PHP:  strrev($s);
来源：http://yl.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://tt.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://yz.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uk.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cz.jianghongdianzi.cn

Ruby: s.reverse
来源：http://gv.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jp.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://qv.panjiajie.cn

Py:   s.count("a")
来源：http://hj.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://ox.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://au.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://yf.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rv.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://bv.panjiajie.cn

Ruby: s.count("a")
来源：http://cd.shtwfgs.cn

C#:   s.Count(c => c == 'a')
来源：http://oa.9csxet.cn

[E13] 逐字符遍历
来源：http://pa.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://ls.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tu.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mm.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vl.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sa.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mj.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://do.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jb.newstarts.cn

[E14] URL 编码与 Base64
来源：http://fq.hahajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ut.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bi.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ae.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ti.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mz.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bl.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cm.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cg.szsharing.cn

[E15] HTML 转义 / 反转义
来源：http://rl.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ta.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jv.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cj.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://to.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nq.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://os.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xo.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ri.hnjuh.cn

[E16] 数字千分位
来源：http://vt.asd995.cn

Py:   f"{1234567:,}"
来源：http://ej.shxzskj.cn

PHP:  number_format(1234567);
来源：http://pi.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://iu.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hq.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://na.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qj.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sh.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://cf.huixiangedu.cn

[E17] 首字母大写
来源：http://hp.shxzskj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cl.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ef.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wt.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xt.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://go.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ob.wgjwhj.cn

Ruby: s.capitalize
来源：http://ba.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yc.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://gk.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ji.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zr.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fv.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nv.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jn.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nw.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lw.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xi.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://kf.chemitech.net.cn

Py:   s.splitlines()
来源：http://dy.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tu.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://yx.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://vl.huixiangedu.cn

Java: s.lines().toList()
来源：http://yi.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://iu.yuntaijiaju.cn

Ruby: s.lines
来源：http://sb.9csxet.cn

C#:   s.Split('\n')
来源：http://fe.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://bl.yuntaijiaju.cn

Py:   if not s:
来源：http://va.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ei.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oz.shtwfgs.cn

TS:   if (s === "") {}
来源：http://oz.huixiangedu.cn

Java: if (s.isEmpty()) {}
来源：http://kl.bookmarksfly.cn

Go:   if s == "" {}
来源：http://pq.szsharing.cn

Ruby: if s.empty?
来源：http://my.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ta.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://pc.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qr.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ms.szsharing.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ve.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jq.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vj.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://po.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zv.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kb.521024.cn

[E22] 字节长度与字符长度
来源：http://gl.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uw.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ku.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xd.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fd.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bz.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tu.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://ux.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dn.jctech888.com.cn

================================================================================
来源：http://zn.szxytkj.cn

F. 文件与目录
来源：http://ph.lnxyls.cn

================================================================================
来源：http://rb.bjjhwx.cn

[F01] 读取整个文件
来源：http://qu.chemitech.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jd.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://um.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sw.muxihuayi.cn


<!-- 参考信息 -->