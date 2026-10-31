代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cq.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hr.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xa.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ot.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yd.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kr.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ee.hahajie.cn

[E02] 重复字符串
来源：http://nq.shtwfgs.cn

Py:   "ab" * 3
来源：http://ud.wgjwhj.cn

PHP:  str_repeat("ab", 3);
来源：http://vs.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://zh.asd995.cn

TS:   "ab".repeat(3)
来源：http://bs.colortex.cn

Java: "ab".repeat(3)
来源：http://oy.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://it.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://om.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vy.521024.cn

[E03] 截取子串
来源：http://tj.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yj.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nw.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rp.huanxung.cn

TS:   s.slice(1, 4)
来源：http://bw.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://ks.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mr.asd995.cn

Ruby: s[1, 3];  s[1..3]
来源：http://at.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://ne.yuexingan06.cn

[E04] 查找子串位置
来源：http://la.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://hv.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://lq.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://om.gzmigu.cn

TS:   s.indexOf("x")
来源：http://hx.huanxung.cn

Java: s.indexOf("x")
来源：http://jq.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://ac.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://hc.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://pd.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ir.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qh.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rt.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qw.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ww.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xf.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ai.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dr.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mt.colortex.cn

[E06] 替换子串
来源：http://gd.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ac.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://ka.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://co.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://sb.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jr.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://py.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lk.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://jg.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://st.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ri.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wf.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ji.yuexingan06.cn

TS:   s.split(",")
来源：http://he.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dh.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tp.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://na.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iv.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://ut.hnjuh.cn

Py:   ",".join(items)
来源：http://ik.szsharing.cn

PHP:  implode(",", $items);
来源：http://pi.bjjhwx.cn

JS:   items.join(",")
来源：http://ce.chemitech.net.cn

TS:   items.join(",")
来源：http://xp.hnjuh.cn

Java: String.join(",", items)
来源：http://do.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://wl.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://ln.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://lt.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://wm.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://db.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ng.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://ja.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://iu.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://mh.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cd.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rj.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oc.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://bw.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ol.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nb.asd995.cn

JS:   "7".padStart(3, "0")
来源：http://ck.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://sw.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://vg.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://iv.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sp.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fr.nicolike.cn

[E11] 反转字符串
来源：http://qp.shtwfgs.cn

Py:   s[::-1]
来源：http://sx.szxytkj.cn

PHP:  strrev($s);
来源：http://sl.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://zh.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://vz.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ei.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hm.wgjwhj.cn

Ruby: s.reverse
来源：http://dy.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zt.newstarts.cn

[E12] 统计某字符出现次数
来源：http://ly.szxytkj.cn

Py:   s.count("a")
来源：http://ot.wgjwhj.cn

PHP:  substr_count($s, "a");
来源：http://zo.521024.cn

JS:   s.split("a").length - 1
来源：http://oq.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://mn.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wp.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://fr.jctech888.com.cn

Ruby: s.count("a")
来源：http://xo.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://fc.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://yl.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://ho.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sa.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xh.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qy.jctech888.com.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ld.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bn.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://aw.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gd.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://lt.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hi.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rf.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dc.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qr.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xf.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rz.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rx.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kr.521024.cn

[E15] HTML 转义 / 反转义
来源：http://jw.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tc.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jy.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zb.hnjuh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nv.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://om.hahajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kd.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zs.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wm.hnjuh.cn

[E16] 数字千分位
来源：http://ll.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://hn.szsharing.cn

PHP:  number_format(1234567);
来源：http://qs.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hl.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ag.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sc.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pt.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uz.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://sg.yuexingan06.cn

[E17] 首字母大写
来源：http://ps.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yn.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rp.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vx.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bw.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://io.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nw.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://zp.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cd.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://kf.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ak.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dj.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bk.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tn.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ky.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://us.hnjuh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cn.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qf.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://oh.shxzukj.cn

Py:   s.splitlines()
来源：http://xb.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kd.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://bi.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://sv.bjjhwx.cn

Java: s.lines().toList()
来源：http://yh.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://cz.nszjky.cn

Ruby: s.lines
来源：http://av.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://fk.asd995.cn

[E20] 判断字符串是否为空
来源：http://ku.szsharing.cn

Py:   if not s:
来源：http://dx.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ft.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://za.muxihuayi.cn

TS:   if (s === "") {}
来源：http://tu.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://sg.newstarts.cn

Go:   if s == "" {}
来源：http://cr.521024.cn

Ruby: if s.empty?
来源：http://lp.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://un.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://xl.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wr.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uq.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gm.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jp.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gn.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://mj.jianghongdianzi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dd.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zz.colortex.cn

[E22] 字节长度与字符长度
来源：http://uw.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lv.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://co.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fb.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qs.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ov.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yj.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://nz.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://op.521024.cn

================================================================================
来源：http://fj.shxzukj.cn

F. 文件与目录
来源：http://ao.muxihuayi.cn

================================================================================
来源：http://qo.wgjwhj.cn

[F01] 读取整个文件
来源：http://gb.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ux.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://ce.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ob.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oy.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://da.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rc.nszjky.cn

Ruby: File.read("a.txt")
来源：http://ml.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://wg.shxzskj.cn

[F02] 逐行读取文件
来源：http://ed.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gf.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sy.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pu.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vn.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ra.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vr.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bm.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rf.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://ap.jianghongdianzi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dv.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ar.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tb.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bc.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zb.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ue.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://la.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nl.yuexingan06.cn

[F04] 追加写入文件
来源：http://nr.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tb.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tf.chemitech.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ud.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://up.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kj.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nt.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jr.shxzukj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ql.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://aw.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qr.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://cm.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://ay.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://mn.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gq.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ho.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://sr.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://vn.yuexingan06.cn

[F06] 删除文件
来源：http://na.wgjwhj.cn

Py:   os.remove("a.txt")
来源：http://ry.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://hf.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://eb.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fm.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jr.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://jw.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://xq.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://br.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://wl.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mh.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fl.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vy.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://la.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pq.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ve.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vn.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cf.shxzukj.cn

[F08] 遍历目录
来源：http://mv.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ji.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xx.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://js.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://vc.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mt.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ex.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://le.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://mc.521024.cn

[F09] 获取文件大小
来源：http://ru.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://bb.9csxet.cn

PHP:  filesize("a.txt");
来源：http://fs.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://ju.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://tw.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hr.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wy.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://qv.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://ps.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://be.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xk.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uh.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gl.colortex.cn

TS:   path.extname("a.txt")
来源：http://vp.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oq.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fk.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ki.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pq.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://sa.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rz.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ug.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ug.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fs.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ap.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bw.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://je.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ar.shxzukj.cn

[F12] CSV 读写
来源：http://fc.szxytkj.cn


<!-- 参考信息 -->