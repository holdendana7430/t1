代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pa.colortex.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ub.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nr.bjjhwx.cn

TS:   [...arr];
来源：http://zn.szsharing.cn

Java: new ArrayList<>(list);
来源：http://go.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yx.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://hv.gzmigu.cn

C#:   new List<int>(list);
来源：http://jd.nicolike.cn

[D23] reduce 累积计算
来源：http://xm.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gp.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hv.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pi.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://md.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pd.shxzukj.cn

Go:   // 手写循环
来源：http://rb.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dg.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iy.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://em.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bn.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bu.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dk.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://po.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gz.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sl.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pu.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sb.bjjhwx.cn

[D25] Set 集合去重与交并差
来源：http://ip.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ap.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ik.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uh.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qd.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vu.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ne.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ya.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oo.asd995.cn

[D26] 数组转字符串
来源：http://dv.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://oj.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://kz.chemitech.net.cn

JS:   arr.join(", ")
来源：http://it.colortex.cn

TS:   arr.join(", ")
来源：http://pa.9csxet.cn

Java: String.join(", ", list)
来源：http://nb.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://xd.gzmigu.cn

Ruby: arr.join(", ")
来源：http://hj.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://yi.hahajie.cn

================================================================================
来源：http://yk.hahajie.cn

E. 字符串处理
来源：http://js.yuntaijiaju.cn

================================================================================
来源：http://kb.shxzukj.cn

[E01] 拼接字符串
来源：http://rh.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gb.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cd.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fs.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ak.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vp.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nl.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xp.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gx.nicolike.cn

[E02] 重复字符串
来源：http://of.colortex.cn

Py:   "ab" * 3
来源：http://xa.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://du.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://wx.newstarts.cn

TS:   "ab".repeat(3)
来源：http://lh.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://gd.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://jd.huixiangedu.cn

Ruby: "ab" * 3
来源：http://yh.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hw.haigaiapp.cn

[E03] 截取子串
来源：http://hx.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gw.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fb.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dq.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://hr.asd995.cn

Java: s.substring(1, 4)
来源：http://is.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cq.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ah.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://to.shxzskj.cn

[E04] 查找子串位置
来源：http://iz.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://li.bjjhwx.cn

PHP:  strpos($s, "x");
来源：http://xf.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tm.nszjky.cn

TS:   s.indexOf("x")
来源：http://cd.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://du.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://rb.gzmigu.cn

Ruby: s.index("x")
来源：http://hc.newstarts.cn

C#:   s.IndexOf("x")
来源：http://go.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fw.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lh.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jh.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gh.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yq.lnxyls.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ds.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mr.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bg.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qo.panjiajie.cn

[E06] 替换子串
来源：http://ju.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xi.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://xe.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nz.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://gh.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://an.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iy.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ys.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://yo.hahajie.cn

[E07] 按分隔符拆分
来源：http://oq.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vx.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://py.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sv.521024.cn

TS:   s.split(",")
来源：http://fk.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kk.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hr.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://rl.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cw.newstarts.cn

[E08] 数组按分隔符合并
来源：http://dq.hnjuh.cn

Py:   ",".join(items)
来源：http://ts.szxytkj.cn

PHP:  implode(",", $items);
来源：http://am.chemitech.net.cn

JS:   items.join(",")
来源：http://in.chemitech.net.cn

TS:   items.join(",")
来源：http://el.lnxyls.cn

Java: String.join(",", items)
来源：http://oq.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://aj.muxihuayi.cn

Ruby: items.join(",")
来源：http://dl.panjiajie.cn

C#:   string.Join(",", items)
来源：http://eu.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://um.shxzukj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ea.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://df.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://dl.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://cq.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://ns.lnxyls.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://in.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qh.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dc.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://vj.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cn.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://il.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://ml.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://ws.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://gc.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://er.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hq.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rr.szsharing.cn

[E11] 反转字符串
来源：http://ra.hnjuh.cn

Py:   s[::-1]
来源：http://ft.panjiajie.cn

PHP:  strrev($s);
来源：http://ty.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://ab.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://ao.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wa.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bo.521024.cn

Ruby: s.reverse
来源：http://mn.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jy.bjjhwx.cn

[E12] 统计某字符出现次数
来源：http://kt.szxytkj.cn

Py:   s.count("a")
来源：http://ut.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://ex.newstarts.cn

JS:   s.split("a").length - 1
来源：http://pb.nszjky.cn

TS:   s.split("a").length - 1
来源：http://dm.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hg.huixinmuqiang.cn

Go:   strings.Count(s, "a")
来源：http://hq.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://sg.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://hd.521024.cn

[E13] 逐字符遍历
来源：http://qc.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://xu.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cl.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lb.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wa.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ik.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cq.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ol.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bg.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://iz.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rm.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://za.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bh.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ul.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hs.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gj.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dn.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gv.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://yy.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://th.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zv.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://em.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ss.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ef.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://en.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bp.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jd.hnjuh.cn

[E16] 数字千分位
来源：http://yo.hahajie.cn

Py:   f"{1234567:,}"
来源：http://gy.newstarts.cn

PHP:  number_format(1234567);
来源：http://ue.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ol.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zj.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://me.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cb.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zh.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://ex.shxzukj.cn

[E17] 首字母大写
来源：http://iq.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://la.shxzskj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xu.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ii.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vc.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://av.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xu.chemitech.net.cn

Ruby: s.capitalize
来源：http://sr.521024.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ai.nszjky.cn

[E18] 模板占位符替换
来源：http://qh.panjiajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sl.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rr.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zm.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mx.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hj.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ax.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iu.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://il.newstarts.cn

[E19] 多行文本按行拆分
来源：http://ip.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://mr.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lb.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://fd.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://cy.asd995.cn

Java: s.lines().toList()
来源：http://vh.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://sv.asd995.cn

Ruby: s.lines
来源：http://ax.hahajie.cn

C#:   s.Split('\n')
来源：http://cu.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://zf.yuntaijiaju.cn

Py:   if not s:
来源：http://ae.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ak.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ia.yuexingan06.cn

TS:   if (s === "") {}
来源：http://fe.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://bq.chemitech.net.cn

Go:   if s == "" {}
来源：http://ur.lnxyls.cn

Ruby: if s.empty?
来源：http://mx.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xx.szxytkj.cn

[E21] 超长截断加省略号
来源：http://kj.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ru.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gb.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gz.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nb.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ee.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://on.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mu.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aq.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://gm.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rd.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jx.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wq.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oy.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gt.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ks.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://ot.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dz.521024.cn

================================================================================
来源：http://go.jctech888.com.cn

F. 文件与目录
来源：http://qm.521024.cn

================================================================================
来源：http://nv.huanxung.cn

[F01] 读取整个文件
来源：http://wh.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://py.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://vk.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cq.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ws.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gr.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bs.nicolike.cn

Ruby: File.read("a.txt")
来源：http://hc.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://gt.shxzukj.cn

[F02] 逐行读取文件
来源：http://oo.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uo.bookmarksfly.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jk.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jy.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://za.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ra.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mi.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qo.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nr.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://ga.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yv.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://iz.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://af.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ag.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pa.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kv.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://re.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vx.bookmarksfly.cn

[F04] 追加写入文件
来源：http://ke.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ia.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wn.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cc.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qq.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rc.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zf.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sw.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cd.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://ks.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nr.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://gn.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://hu.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://rq.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://du.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://na.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://yr.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://ys.haigaiapp.cn

[F06] 删除文件
来源：http://gi.colortex.cn

Py:   os.remove("a.txt")
来源：http://ie.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://us.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pz.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jn.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dl.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://us.hahajie.cn


<!-- 参考信息 -->