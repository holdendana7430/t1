代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vp.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jm.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hp.asd995.cn

[D26] 数组转字符串
来源：http://bd.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://eo.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://xr.521024.cn

JS:   arr.join(", ")
来源：http://yt.nicolike.cn

TS:   arr.join(", ")
来源：http://zo.asd995.cn

Java: String.join(", ", list)
来源：http://qv.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://zr.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://tz.hahajie.cn

C#:   string.Join(", ", list)
来源：http://gb.nicolike.cn

================================================================================
来源：http://ko.521024.cn

E. 字符串处理
来源：http://hj.shtwfgs.cn

================================================================================
来源：http://xf.shxzukj.cn

[E01] 拼接字符串
来源：http://dh.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xs.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://aj.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vp.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zo.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cm.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uk.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mh.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wa.bookmarksfly.cn

[E02] 重复字符串
来源：http://eu.shxzskj.cn

Py:   "ab" * 3
来源：http://jz.jctech888.com.cn

PHP:  str_repeat("ab", 3);
来源：http://ok.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://nd.521024.cn

TS:   "ab".repeat(3)
来源：http://xd.hnjuh.cn

Java: "ab".repeat(3)
来源：http://ky.wgjwhj.cn

Go:   strings.Repeat("ab", 3)
来源：http://ub.newstarts.cn

Ruby: "ab" * 3
来源：http://wi.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sc.huixinmuqiang.cn

[E03] 截取子串
来源：http://sm.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bo.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ns.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://su.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://uf.nicolike.cn

Java: s.substring(1, 4)
来源：http://tz.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hp.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pe.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://ne.wgjwhj.cn

[E04] 查找子串位置
来源：http://im.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://wg.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://ab.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oa.nszjky.cn

TS:   s.indexOf("x")
来源：http://ad.gzmigu.cn

Java: s.indexOf("x")
来源：http://ay.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://nx.muxihuayi.cn

Ruby: s.index("x")
来源：http://zl.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://zl.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ee.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jg.colortex.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cb.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ml.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ui.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wf.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tb.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xi.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pk.9csxet.cn

[E06] 替换子串
来源：http://nk.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://he.huanxung.cn

PHP:  str_replace("a", "b", $s);
来源：http://sq.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pf.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://zn.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ox.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vi.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lw.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://cq.colortex.cn

[E07] 按分隔符拆分
来源：http://sc.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fs.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rg.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xz.jianghongdianzi.cn

TS:   s.split(",")
来源：http://xt.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mv.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yw.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://di.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://za.newstarts.cn

[E08] 数组按分隔符合并
来源：http://xw.newstarts.cn

Py:   ",".join(items)
来源：http://uu.colortex.cn

PHP:  implode(",", $items);
来源：http://pc.bjjhwx.cn

JS:   items.join(",")
来源：http://zv.huixinmuqiang.cn

TS:   items.join(",")
来源：http://gd.colortex.cn

Java: String.join(",", items)
来源：http://gg.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://ve.huanxung.cn

Ruby: items.join(",")
来源：http://vn.newstarts.cn

C#:   string.Join(",", items)
来源：http://eg.huanxung.cn

[E09] 去除所有空白字符
来源：http://tw.shxzukj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ql.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://op.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://sh.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://pp.jianghongdianzi.cn

Java: s.replaceAll("\\s+", "")
来源：http://yp.gzmigu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cd.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://eu.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dh.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://bc.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yt.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mn.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://sx.521024.cn

TS:   "7".padStart(3, "0")
来源：http://ks.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://il.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tw.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dc.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://la.hnjuh.cn

[E11] 反转字符串
来源：http://hi.jianghongdianzi.cn

Py:   s[::-1]
来源：http://wa.521024.cn

PHP:  strrev($s);
来源：http://vc.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://ia.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://cz.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lo.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://iz.haigaiapp.cn

Ruby: s.reverse
来源：http://pj.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pz.521024.cn

[E12] 统计某字符出现次数
来源：http://iz.9csxet.cn

Py:   s.count("a")
来源：http://fn.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://rn.huanxung.cn

JS:   s.split("a").length - 1
来源：http://qy.colortex.cn

TS:   s.split("a").length - 1
来源：http://ha.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ew.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://ld.szsharing.cn

Ruby: s.count("a")
来源：http://pz.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://ub.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://wk.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://zv.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cx.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jx.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zc.huixiangedu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bd.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tk.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sq.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xk.asd995.cn

[E14] URL 编码与 Base64
来源：http://sd.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qx.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ng.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dz.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://up.bjjhwx.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yh.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dn.jctech888.com.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sb.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ld.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://ti.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hx.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://el.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yu.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dp.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fj.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xp.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mz.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xi.yuntaijiaju.cn

[E16] 数字千分位
来源：http://ha.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://xe.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://dz.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mf.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ki.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gx.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xd.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ch.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://le.panjiajie.cn

[E17] 首字母大写
来源：http://ja.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jg.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hw.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uz.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cb.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rp.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gp.jctech888.com.cn

Ruby: s.capitalize
来源：http://su.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ay.newstarts.cn

[E18] 模板占位符替换
来源：http://fd.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gb.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wk.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ug.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mn.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://om.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bi.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ce.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kd.nszjky.cn

[E19] 多行文本按行拆分
来源：http://nh.muxihuayi.cn

Py:   s.splitlines()
来源：http://ar.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://va.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://wn.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://pw.shxzukj.cn

Java: s.lines().toList()
来源：http://hl.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://ir.szsharing.cn

Ruby: s.lines
来源：http://jw.wgjwhj.cn

C#:   s.Split('\n')
来源：http://bp.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://cy.shxzskj.cn

Py:   if not s:
来源：http://cv.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://je.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://my.9csxet.cn

TS:   if (s === "") {}
来源：http://cu.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://wt.chemitech.net.cn

Go:   if s == "" {}
来源：http://ow.gzmigu.cn

Ruby: if s.empty?
来源：http://bz.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://et.huanxung.cn

[E21] 超长截断加省略号
来源：http://wo.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dq.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sp.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ao.colortex.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qe.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qr.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://ny.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uq.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://te.hahajie.cn

[E22] 字节长度与字符长度
来源：http://ig.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://up.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qn.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zj.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pw.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xf.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eo.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://nq.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ii.muxihuayi.cn

================================================================================
来源：http://jw.nicolike.cn

F. 文件与目录
来源：http://pd.gzmigu.cn

================================================================================
来源：http://kl.huanxung.cn

[F01] 读取整个文件
来源：http://ue.chemitech.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://er.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://az.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cd.muxihuayi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lr.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wi.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ik.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://vq.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://rf.bjjhwx.cn

[F02] 逐行读取文件
来源：http://zb.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dc.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bo.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xk.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xd.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lu.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qc.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gx.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ah.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://fs.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gc.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ve.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iw.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jc.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kj.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yf.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://hw.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ze.bjjhwx.cn

[F04] 追加写入文件
来源：http://nm.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://re.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iu.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uo.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yg.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pg.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ow.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xe.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cv.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://dd.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://km.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://gl.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://uq.yuntaijiaju.cn

TS:   fs.existsSync("a.txt")
来源：http://mx.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cu.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hu.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://lu.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://bf.shtwfgs.cn

[F06] 删除文件
来源：http://jd.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://qu.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://uz.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lr.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ly.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nt.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://fs.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://sp.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://iq.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://ym.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://io.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yk.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sk.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xg.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sw.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xd.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://of.huanxung.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ro.haigaiapp.cn

[F08] 遍历目录
来源：http://ky.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yl.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zw.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://fa.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://dk.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hd.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tv.huixiangedu.cn

Ruby: Dir.children("dir")
来源：http://vq.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://he.shxzskj.cn

[F09] 获取文件大小
来源：http://lt.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://qt.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://vs.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://fz.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://zm.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qt.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sh.nicolike.cn

Ruby: File.size("a.txt")
来源：http://gw.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://ra.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://vp.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kr.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mg.nszjky.cn


<!-- 参考信息 -->