代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fa.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://yu.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fi.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ie.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fh.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bw.shxzukj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kl.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oq.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jd.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dq.asd995.cn

[D25] Set 集合去重与交并差
来源：http://hr.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jw.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wl.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gz.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sr.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oh.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pp.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ys.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://to.newstarts.cn

[D26] 数组转字符串
来源：http://xc.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://md.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://rs.panjiajie.cn

JS:   arr.join(", ")
来源：http://kd.jctech888.com.cn

TS:   arr.join(", ")
来源：http://gd.szsharing.cn

Java: String.join(", ", list)
来源：http://jh.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://if.hnjuh.cn

Ruby: arr.join(", ")
来源：http://ix.huanxung.cn

C#:   string.Join(", ", list)
来源：http://ru.huixiangedu.cn

================================================================================
来源：http://qo.colortex.cn

E. 字符串处理
来源：http://wi.yuntaijiaju.cn

================================================================================
来源：http://of.huanxung.cn

[E01] 拼接字符串
来源：http://wo.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rm.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ep.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tx.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gr.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vb.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mh.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rt.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rn.nszjky.cn

[E02] 重复字符串
来源：http://su.bjjhwx.cn

Py:   "ab" * 3
来源：http://op.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://hp.szsharing.cn

JS:   "ab".repeat(3)
来源：http://xn.newstarts.cn

TS:   "ab".repeat(3)
来源：http://dt.nicolike.cn

Java: "ab".repeat(3)
来源：http://za.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://uk.muxihuayi.cn

Ruby: "ab" * 3
来源：http://jw.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vj.huixinmuqiang.cn

[E03] 截取子串
来源：http://jw.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yo.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kx.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ja.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://qx.521024.cn

Java: s.substring(1, 4)
来源：http://hw.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://py.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://la.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://kx.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://wd.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://ua.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://qh.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wh.shxzskj.cn

TS:   s.indexOf("x")
来源：http://kt.panjiajie.cn

Java: s.indexOf("x")
来源：http://cd.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://vb.jctech888.com.cn

Ruby: s.index("x")
来源：http://qp.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://le.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xl.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sw.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ut.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zp.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://im.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://in.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dq.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kh.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bm.hahajie.cn

[E06] 替换子串
来源：http://en.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iw.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://pt.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sm.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://mq.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jj.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ep.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bh.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://th.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://qs.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ob.nicolike.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yt.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ti.szxytkj.cn

TS:   s.split(",")
来源：http://li.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bl.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://og.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://jv.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ii.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://vt.yuexingan06.cn

Py:   ",".join(items)
来源：http://vn.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://ws.shxzukj.cn

JS:   items.join(",")
来源：http://qn.shtwfgs.cn

TS:   items.join(",")
来源：http://ev.shtwfgs.cn

Java: String.join(",", items)
来源：http://id.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://dv.shxzukj.cn

Ruby: items.join(",")
来源：http://go.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://ff.hnjuh.cn

[E09] 去除所有空白字符
来源：http://jk.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qg.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ei.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://kc.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://jl.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://ox.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zo.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gy.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vg.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://ff.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jx.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://az.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://cy.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://tc.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://kt.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fn.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wj.yuexingan06.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bt.huanxung.cn

[E11] 反转字符串
来源：http://mx.yuntaijiaju.cn

Py:   s[::-1]
来源：http://cc.panjiajie.cn

PHP:  strrev($s);
来源：http://ly.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://cg.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://xw.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nz.yuexingan06.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cw.chemitech.net.cn

Ruby: s.reverse
来源：http://py.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vu.nicolike.cn

[E12] 统计某字符出现次数
来源：http://su.colortex.cn

Py:   s.count("a")
来源：http://yu.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://dc.asd995.cn

JS:   s.split("a").length - 1
来源：http://ny.9csxet.cn

TS:   s.split("a").length - 1
来源：http://oq.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ez.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://wk.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://iw.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://fs.521024.cn

[E13] 逐字符遍历
来源：http://ih.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://dt.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zf.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sz.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zy.hahajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rw.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qz.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yu.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xy.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://ra.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pt.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yp.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kn.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wd.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gw.asd995.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rs.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vu.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ry.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://th.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mh.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bh.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://os.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ce.huanxung.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uq.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rz.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fm.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ef.521024.cn

[E16] 数字千分位
来源：http://iq.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://ex.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://cq.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bz.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ts.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pp.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ka.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jz.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://es.521024.cn

[E17] 首字母大写
来源：http://mi.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cq.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bu.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jh.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jo.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pq.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nv.szxytkj.cn

Ruby: s.capitalize
来源：http://ed.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cr.hahajie.cn

[E18] 模板占位符替换
来源：http://gx.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nw.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xw.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hr.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vx.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jh.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ql.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lg.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://de.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://mp.haigaiapp.cn

Py:   s.splitlines()
来源：http://pg.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dv.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://we.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://du.haigaiapp.cn

Java: s.lines().toList()
来源：http://er.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://tv.gzmigu.cn

Ruby: s.lines
来源：http://ha.nicolike.cn

C#:   s.Split('\n')
来源：http://zq.9csxet.cn

[E20] 判断字符串是否为空
来源：http://aa.521024.cn

Py:   if not s:
来源：http://qx.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nx.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wg.chemitech.net.cn

TS:   if (s === "") {}
来源：http://vo.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://od.jctech888.com.cn

Go:   if s == "" {}
来源：http://gq.9csxet.cn

Ruby: if s.empty?
来源：http://iw.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fd.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://bk.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ay.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kz.szsharing.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yc.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mb.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dr.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://et.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ar.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dz.nicolike.cn

[E22] 字节长度与字符长度
来源：http://za.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qy.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gj.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nn.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nv.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kb.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bn.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://sl.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zx.asd995.cn

================================================================================
来源：http://yz.wgjwhj.cn

F. 文件与目录
来源：http://ki.haigaiapp.cn

================================================================================
来源：http://aw.9csxet.cn

[F01] 读取整个文件
来源：http://ic.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ba.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://zr.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nt.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mt.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jr.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qo.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://ut.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://ox.nszjky.cn

[F02] 逐行读取文件
来源：http://xb.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gc.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vh.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://va.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vy.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ly.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yf.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ld.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sx.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://gm.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wf.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bc.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ep.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jf.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lc.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fh.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://ce.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tk.521024.cn

[F04] 追加写入文件
来源：http://io.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lc.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qz.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://im.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yp.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ht.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rg.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://di.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://px.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://yw.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ew.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://wt.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://vf.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://ez.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ts.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://he.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://ww.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://vw.shtwfgs.cn

[F06] 删除文件
来源：http://tl.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://sa.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://kk.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zp.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rs.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ei.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://ze.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://af.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://cc.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://bd.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sx.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dy.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dc.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cp.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tj.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://do.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vm.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xd.jianghongdianzi.cn

[F08] 遍历目录
来源：http://rn.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jo.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fy.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://rj.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://rj.haigaiapp.cn


<!-- 参考信息 -->