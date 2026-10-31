代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://yl.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://lk.colortex.cn

JS:   arr.join(", ")
来源：http://yq.nicolike.cn

TS:   arr.join(", ")
来源：http://yk.asd995.cn

Java: String.join(", ", list)
来源：http://xc.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://vc.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://gr.nszjky.cn

C#:   string.Join(", ", list)
来源：http://cv.hnjuh.cn

================================================================================
来源：http://bx.bjjhwx.cn

E. 字符串处理
来源：http://qq.asd995.cn

================================================================================
来源：http://jo.huanxung.cn

[E01] 拼接字符串
来源：http://rf.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ay.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mf.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hc.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://as.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nc.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://al.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bj.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jm.panjiajie.cn

[E02] 重复字符串
来源：http://gn.huixiangedu.cn

Py:   "ab" * 3
来源：http://jp.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://ek.9csxet.cn

JS:   "ab".repeat(3)
来源：http://es.huanxung.cn

TS:   "ab".repeat(3)
来源：http://zl.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://yj.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://uy.gzmigu.cn

Ruby: "ab" * 3
来源：http://oi.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yt.asd995.cn

[E03] 截取子串
来源：http://dg.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://td.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fs.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dx.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://ji.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://mr.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ei.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://px.colortex.cn

C#:   s.Substring(1, 3)
来源：http://jn.hnjuh.cn

[E04] 查找子串位置
来源：http://mv.szsharing.cn

Py:   s.find("x");  s.index("x")
来源：http://je.colortex.cn

PHP:  strpos($s, "x");
来源：http://mv.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://zm.hnjuh.cn

Java: s.indexOf("x")
来源：http://xm.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://yk.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://pg.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://lu.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://by.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qk.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ej.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mu.hahajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yv.wgjwhj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ra.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wm.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ny.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://em.bookmarksfly.cn

[E06] 替换子串
来源：http://on.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ng.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://ud.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zg.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://sz.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nq.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yk.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sg.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://vo.lnxyls.cn

[E07] 按分隔符拆分
来源：http://os.newstarts.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pt.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ku.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mp.shtwfgs.cn

TS:   s.split(",")
来源：http://ua.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jr.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ix.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://sm.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dh.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://hc.szsharing.cn

Py:   ",".join(items)
来源：http://ry.hahajie.cn

PHP:  implode(",", $items);
来源：http://gl.shxzskj.cn

JS:   items.join(",")
来源：http://sd.panjiajie.cn

TS:   items.join(",")
来源：http://od.szxytkj.cn

Java: String.join(",", items)
来源：http://ff.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://at.jctech888.com.cn

Ruby: items.join(",")
来源：http://sj.shxzskj.cn

C#:   string.Join(",", items)
来源：http://eu.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://pq.shxzukj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ox.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bo.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://zn.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://xs.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://ea.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ut.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qs.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jf.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://jy.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cd.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pl.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://im.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://fv.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://fn.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tg.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://op.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fg.szxytkj.cn

[E11] 反转字符串
来源：http://wg.asd995.cn

Py:   s[::-1]
来源：http://lx.nicolike.cn

PHP:  strrev($s);
来源：http://so.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://eq.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://ml.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yc.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zm.jianghongdianzi.cn

Ruby: s.reverse
来源：http://uh.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nz.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://px.shxzukj.cn

Py:   s.count("a")
来源：http://db.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://kb.521024.cn

JS:   s.split("a").length - 1
来源：http://xf.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://vk.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://au.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://jq.lnxyls.cn

Ruby: s.count("a")
来源：http://xr.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://ka.bjjhwx.cn

[E13] 逐字符遍历
来源：http://lh.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://qv.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bh.gzmigu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wz.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bf.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://of.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dq.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uq.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zg.nszjky.cn

[E14] URL 编码与 Base64
来源：http://is.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aj.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vw.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yd.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bb.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fv.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tn.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sa.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uh.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://ng.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ul.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ws.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oa.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://uc.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bc.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hi.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wl.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gi.9csxet.cn

[E16] 数字千分位
来源：http://dn.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://ol.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://ak.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vz.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://iq.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iq.gzmigu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://us.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qr.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://os.huixiangedu.cn

[E17] 首字母大写
来源：http://zm.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ly.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tq.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hp.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ai.nicolike.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sk.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pu.shxzskj.cn

Ruby: s.capitalize
来源：http://fv.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pb.yuexingan06.cn

[E18] 模板占位符替换
来源：http://yv.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sh.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nc.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lr.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gs.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dn.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://my.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vl.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pv.521024.cn

[E19] 多行文本按行拆分
来源：http://ox.szsharing.cn

Py:   s.splitlines()
来源：http://mt.yuntaijiaju.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ke.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://hx.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://fr.colortex.cn

Java: s.lines().toList()
来源：http://lk.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://ym.gzmigu.cn

Ruby: s.lines
来源：http://ei.szsharing.cn

C#:   s.Split('\n')
来源：http://fj.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://xn.chemitech.net.cn

Py:   if not s:
来源：http://na.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qj.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jv.hahajie.cn

TS:   if (s === "") {}
来源：http://tu.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://wq.521024.cn

Go:   if s == "" {}
来源：http://ep.huixiangedu.cn

Ruby: if s.empty?
来源：http://su.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yo.shxzskj.cn

[E21] 超长截断加省略号
来源：http://bo.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hd.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gh.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gd.colortex.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aa.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://if.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://vu.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hx.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vc.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://gn.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ao.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ve.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://im.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ne.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://am.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sa.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://nd.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fj.521024.cn

================================================================================
来源：http://xh.bookmarksfly.cn

F. 文件与目录
来源：http://fx.yuexingan06.cn

================================================================================
来源：http://sw.newstarts.cn

[F01] 读取整个文件
来源：http://vs.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rg.yuntaijiaju.cn

PHP:  file_get_contents("a.txt");
来源：http://wc.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hs.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bz.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ry.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nd.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://lh.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://ix.newstarts.cn

[F02] 逐行读取文件
来源：http://ds.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ow.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ju.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://la.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qa.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pj.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://el.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ct.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://te.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://yn.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wc.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://is.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mf.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bt.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://my.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mv.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://xp.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qw.asd995.cn

[F04] 追加写入文件
来源：http://rw.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cq.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ab.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cd.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bd.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zd.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fm.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://al.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gj.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://kk.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vi.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://pd.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://ck.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://ki.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gi.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qf.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://aa.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://ld.nicolike.cn

[F06] 删除文件
来源：http://kj.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://sv.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://jk.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bn.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://de.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://em.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://uy.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://lw.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://qp.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://kg.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xb.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bh.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fe.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yf.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ee.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ah.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dk.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ia.nicolike.cn

[F08] 遍历目录
来源：http://jc.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wn.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rj.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://rn.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://gk.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kl.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hy.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://fq.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://gq.haigaiapp.cn

[F09] 获取文件大小
来源：http://mm.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://sn.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://kk.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://mt.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://js.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hr.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mf.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://wn.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://cf.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://ax.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iq.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ij.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://il.newstarts.cn

TS:   path.extname("a.txt")
来源：http://tw.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rx.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sc.haigaiapp.cn


<!-- 参考信息 -->