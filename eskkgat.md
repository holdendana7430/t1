代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aj.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://un.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jy.gzmigu.cn

TS:   [...arr];
来源：http://ja.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://wd.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gi.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://ah.bookmarksfly.cn

C#:   new List<int>(list);
来源：http://tw.colortex.cn

[D23] reduce 累积计算
来源：http://zh.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vm.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ij.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xs.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lv.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ik.panjiajie.cn

Go:   // 手写循环
来源：http://wk.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gr.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ck.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://yf.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nl.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ob.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ii.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kw.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kf.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cv.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ag.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ai.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://md.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qf.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ia.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xa.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ra.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hv.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zp.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zi.jianghongdianzi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dr.shxzskj.cn

[D26] 数组转字符串
来源：http://sp.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://vh.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://va.hahajie.cn

JS:   arr.join(", ")
来源：http://ta.gzmigu.cn

TS:   arr.join(", ")
来源：http://zw.szxytkj.cn

Java: String.join(", ", list)
来源：http://up.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://tk.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://ec.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://sh.bjjhwx.cn

================================================================================
来源：http://jq.9csxet.cn

E. 字符串处理
来源：http://xm.asd995.cn

================================================================================
来源：http://pb.newstarts.cn

[E01] 拼接字符串
来源：http://te.521024.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ii.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jl.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sv.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ee.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hq.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bo.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ah.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uv.panjiajie.cn

[E02] 重复字符串
来源：http://mi.asd995.cn

Py:   "ab" * 3
来源：http://eg.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://lo.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://bw.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://xb.9csxet.cn

Java: "ab".repeat(3)
来源：http://cf.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://oy.bjjhwx.cn

Ruby: "ab" * 3
来源：http://ud.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kf.gzmigu.cn

[E03] 截取子串
来源：http://ug.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wq.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://au.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ag.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://vm.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://ks.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pb.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gs.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://sr.jctech888.com.cn

[E04] 查找子串位置
来源：http://km.szsharing.cn

Py:   s.find("x");  s.index("x")
来源：http://hu.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://oc.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ei.szxytkj.cn

TS:   s.indexOf("x")
来源：http://je.newstarts.cn

Java: s.indexOf("x")
来源：http://yj.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://gg.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://jo.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://zo.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sc.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rn.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ai.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oi.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ay.colortex.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oz.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wl.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gq.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ob.gzmigu.cn

[E06] 替换子串
来源：http://rd.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iv.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://py.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yg.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://ne.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://or.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fr.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ds.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://yn.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://fx.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rn.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wf.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://br.9csxet.cn

TS:   s.split(",")
来源：http://vz.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://in.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zj.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://nn.panjiajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rp.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://qi.szxytkj.cn

Py:   ",".join(items)
来源：http://mo.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://rj.wgjwhj.cn

JS:   items.join(",")
来源：http://bf.shxzskj.cn

TS:   items.join(",")
来源：http://tq.szxytkj.cn

Java: String.join(",", items)
来源：http://sc.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://vl.haigaiapp.cn

Ruby: items.join(",")
来源：http://qf.nicolike.cn

C#:   string.Join(",", items)
来源：http://rh.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://mt.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gq.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sg.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://nz.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://qk.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://aj.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cy.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ut.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jz.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://iw.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pp.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ac.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://xy.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://un.szsharing.cn

Java: String.format("%03d", 7)
来源：http://cj.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fe.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ct.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bq.shxzskj.cn

[E11] 反转字符串
来源：http://pw.colortex.cn

Py:   s[::-1]
来源：http://ri.nicolike.cn

PHP:  strrev($s);
来源：http://qc.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://ma.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://yz.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zp.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mi.panjiajie.cn

Ruby: s.reverse
来源：http://kq.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kn.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://ov.lnxyls.cn

Py:   s.count("a")
来源：http://yt.521024.cn

PHP:  substr_count($s, "a");
来源：http://ap.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://px.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://sp.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fr.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://ui.haigaiapp.cn

Ruby: s.count("a")
来源：http://ch.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://wi.haigaiapp.cn

[E13] 逐字符遍历
来源：http://sx.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://mi.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kh.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tg.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pq.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vr.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kv.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hs.lnxyls.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://av.huanxung.cn

[E14] URL 编码与 Base64
来源：http://jz.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cz.jctech888.com.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://oo.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fd.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ot.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mf.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cv.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://um.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nr.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://vh.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lk.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mw.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ya.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bf.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://at.hahajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ok.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tu.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qs.szxytkj.cn

[E16] 数字千分位
来源：http://eu.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://tv.lnxyls.cn

PHP:  number_format(1234567);
来源：http://zj.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ws.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ht.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nd.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qv.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mr.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://df.nicolike.cn

[E17] 首字母大写
来源：http://xg.shxzskj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nz.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kx.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kd.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dy.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dh.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qd.szxytkj.cn

Ruby: s.capitalize
来源：http://ep.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rz.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://dx.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eb.gzmigu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aa.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qw.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ma.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bn.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lb.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vb.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yv.521024.cn

[E19] 多行文本按行拆分
来源：http://ux.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://wt.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hx.panjiajie.cn

JS:   s.split(/\r?\n/)
来源：http://uc.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://nj.hnjuh.cn

Java: s.lines().toList()
来源：http://aq.hnjuh.cn

Go:   strings.Split(s, "\n")
来源：http://ui.gzmigu.cn

Ruby: s.lines
来源：http://lc.lnxyls.cn

C#:   s.Split('\n')
来源：http://oj.huanxung.cn

[E20] 判断字符串是否为空
来源：http://fw.wgjwhj.cn

Py:   if not s:
来源：http://fk.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://as.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ak.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://pd.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://wj.jctech888.com.cn

Go:   if s == "" {}
来源：http://ko.wgjwhj.cn

Ruby: if s.empty?
来源：http://ua.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vd.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://nj.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dq.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ur.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qx.hnjuh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ho.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fj.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://wn.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://et.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ma.huanxung.cn

[E22] 字节长度与字符长度
来源：http://ts.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xw.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://al.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bm.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ba.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mg.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kb.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://oc.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bk.wgjwhj.cn

================================================================================
来源：http://ix.huanxung.cn

F. 文件与目录
来源：http://au.muxihuayi.cn

================================================================================
来源：http://up.colortex.cn

[F01] 读取整个文件
来源：http://bs.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fh.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://am.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zn.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://td.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kw.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oo.szsharing.cn

Ruby: File.read("a.txt")
来源：http://pu.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://cg.huixiangedu.cn

[F02] 逐行读取文件
来源：http://eo.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jz.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hn.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iv.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hx.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ty.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dt.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wo.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wu.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://li.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://an.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ya.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jp.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://my.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bh.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vt.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://ci.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pv.huixiangedu.cn

[F04] 追加写入文件
来源：http://jl.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rv.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zs.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yt.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vp.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tu.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dv.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ji.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pg.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://hj.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mm.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://ek.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://yz.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://rw.lnxyls.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kl.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rd.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://kk.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://kk.jianghongdianzi.cn

[F06] 删除文件
来源：http://xg.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://hs.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://tn.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wu.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ae.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gf.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://dp.hnjuh.cn


<!-- 参考信息 -->