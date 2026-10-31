代发 wailian999

================================================================================
来源：http://dr.szsharing.cn

E. 字符串处理
来源：http://sd.asd995.cn

================================================================================
来源：http://lg.shxzskj.cn

[E01] 拼接字符串
来源：http://fd.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://en.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rh.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hx.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xi.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xr.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ra.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://on.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://av.yuntaijiaju.cn

[E02] 重复字符串
来源：http://zm.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://dx.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://oe.asd995.cn

JS:   "ab".repeat(3)
来源：http://ty.nszjky.cn

TS:   "ab".repeat(3)
来源：http://lt.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://fl.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://ph.shxzskj.cn

Ruby: "ab" * 3
来源：http://du.gzmigu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sp.newstarts.cn

[E03] 截取子串
来源：http://cv.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pw.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zd.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fu.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://zb.szxytkj.cn

Java: s.substring(1, 4)
来源：http://jl.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hq.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xg.nszjky.cn

C#:   s.Substring(1, 3)
来源：http://gh.521024.cn

[E04] 查找子串位置
来源：http://vy.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://ge.521024.cn

PHP:  strpos($s, "x");
来源：http://au.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yf.nszjky.cn

TS:   s.indexOf("x")
来源：http://ua.yuexingan06.cn

Java: s.indexOf("x")
来源：http://ho.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://tj.shxzukj.cn

Ruby: s.index("x")
来源：http://fs.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://aw.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ts.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ge.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yi.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hw.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mo.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mk.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qo.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pg.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wm.haigaiapp.cn

[E06] 替换子串
来源：http://qz.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xv.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://mq.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dj.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://yi.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pn.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tv.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://az.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://ol.521024.cn

[E07] 按分隔符拆分
来源：http://gc.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ge.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fw.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ym.szxytkj.cn

TS:   s.split(",")
来源：http://cn.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wp.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ox.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://ud.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wd.nszjky.cn

[E08] 数组按分隔符合并
来源：http://nw.bookmarksfly.cn

Py:   ",".join(items)
来源：http://sf.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://iw.panjiajie.cn

JS:   items.join(",")
来源：http://do.yuntaijiaju.cn

TS:   items.join(",")
来源：http://gt.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://eu.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://nk.szxytkj.cn

Ruby: items.join(",")
来源：http://kr.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://ph.shxzskj.cn

[E09] 去除所有空白字符
来源：http://om.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gp.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://it.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://mi.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://tx.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://gu.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vs.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cx.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ux.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://lq.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lz.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ca.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://ef.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://oc.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://ll.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ge.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ua.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://so.9csxet.cn

[E11] 反转字符串
来源：http://pz.wgjwhj.cn

Py:   s[::-1]
来源：http://fm.521024.cn

PHP:  strrev($s);
来源：http://ut.asd995.cn

JS:   [...s].reverse().join("")
来源：http://tp.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://hu.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://is.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bk.jctech888.com.cn

Ruby: s.reverse
来源：http://ik.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fn.9csxet.cn

[E12] 统计某字符出现次数
来源：http://vj.huixiangedu.cn

Py:   s.count("a")
来源：http://bj.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://yw.huanxung.cn

JS:   s.split("a").length - 1
来源：http://hh.yuexingan06.cn

TS:   s.split("a").length - 1
来源：http://nb.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wb.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://qf.colortex.cn

Ruby: s.count("a")
来源：http://kf.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://md.asd995.cn

[E13] 逐字符遍历
来源：http://lg.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://wn.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nh.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://st.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nb.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ff.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bx.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bb.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rx.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://sn.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qq.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qb.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wz.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gi.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uy.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pk.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vo.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lj.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://qk.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rb.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cr.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yj.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sp.hnjuh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rq.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ut.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://to.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wk.nicolike.cn

[E16] 数字千分位
来源：http://ba.9csxet.cn

Py:   f"{1234567:,}"
来源：http://ua.szxytkj.cn

PHP:  number_format(1234567);
来源：http://bf.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ja.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kc.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hy.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gc.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://my.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://hv.chemitech.net.cn

[E17] 首字母大写
来源：http://ji.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wr.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mh.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fg.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gm.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lt.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://of.haigaiapp.cn

Ruby: s.capitalize
来源：http://nm.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ih.yuexingan06.cn

[E18] 模板占位符替换
来源：http://kt.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://me.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zj.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ol.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cy.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ct.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://az.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yp.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uc.szsharing.cn

[E19] 多行文本按行拆分
来源：http://kb.colortex.cn

Py:   s.splitlines()
来源：http://om.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dl.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://cx.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://lk.yuexingan06.cn

Java: s.lines().toList()
来源：http://ki.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://jy.nicolike.cn

Ruby: s.lines
来源：http://ss.lnxyls.cn

C#:   s.Split('\n')
来源：http://kz.521024.cn

[E20] 判断字符串是否为空
来源：http://xq.521024.cn

Py:   if not s:
来源：http://tz.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nk.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yi.gzmigu.cn

TS:   if (s === "") {}
来源：http://uk.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://qe.chemitech.net.cn

Go:   if s == "" {}
来源：http://zd.bjjhwx.cn

Ruby: if s.empty?
来源：http://up.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pf.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://eh.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pc.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://of.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vk.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gj.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ka.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://ug.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://at.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bt.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://kr.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zz.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ws.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uv.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://av.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cn.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://on.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://so.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ik.haigaiapp.cn

================================================================================
来源：http://jy.panjiajie.cn

F. 文件与目录
来源：http://fm.shxzskj.cn

================================================================================
来源：http://mv.yuexingan06.cn

[F01] 读取整个文件
来源：http://we.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gs.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://cw.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tc.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ta.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lr.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jq.newstarts.cn

Ruby: File.read("a.txt")
来源：http://tq.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://yn.szxytkj.cn

[F02] 逐行读取文件
来源：http://ss.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://we.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ps.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xg.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fa.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nd.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mw.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qn.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ka.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://kh.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zd.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fn.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hl.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zw.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bp.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wg.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://ge.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dy.huixiangedu.cn

[F04] 追加写入文件
来源：http://zn.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ix.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qy.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jo.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kr.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kx.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uv.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vg.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://we.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://dc.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bm.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://lz.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://ok.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://jz.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tl.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://im.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://rd.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://lb.muxihuayi.cn

[F06] 删除文件
来源：http://ah.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://sq.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://no.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ba.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vl.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rb.521024.cn

Go:   os.Remove("a.txt")
来源：http://we.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://vi.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://tp.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://mh.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jb.shtwfgs.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mi.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ta.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bi.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dc.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oj.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cw.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qk.wgjwhj.cn

[F08] 遍历目录
来源：http://fz.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vm.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hb.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://oy.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://ya.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://te.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://um.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://vt.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://ps.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://rq.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://wq.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://zs.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://xz.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://aw.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pl.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zv.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://rv.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://cn.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://xw.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ke.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rx.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://go.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://qu.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ki.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tr.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gc.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iq.huixiangedu.cn

[F11] 复制与移动文件
来源：http://xv.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ud.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://va.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mq.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ss.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wi.haigaiapp.cn


<!-- 参考信息 -->