代发 wailian999

Java: String.join(", ", list)
来源：http://bh.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://eb.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://lk.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://ka.yuexingan06.cn

================================================================================
来源：http://hs.bjjhwx.cn

E. 字符串处理
来源：http://ly.wgjwhj.cn

================================================================================
来源：http://ep.colortex.cn

[E01] 拼接字符串
来源：http://lr.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pg.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kl.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vo.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://to.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fm.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ym.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pv.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nc.jianghongdianzi.cn

[E02] 重复字符串
来源：http://ya.shxzskj.cn

Py:   "ab" * 3
来源：http://ya.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://tt.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://ut.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://ah.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://ku.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://ok.bjjhwx.cn

Ruby: "ab" * 3
来源：http://wb.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xw.jianghongdianzi.cn

[E03] 截取子串
来源：http://yl.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ny.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://be.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sv.9csxet.cn

TS:   s.slice(1, 4)
来源：http://ct.szsharing.cn

Java: s.substring(1, 4)
来源：http://jx.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vr.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mu.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://hb.szxytkj.cn

[E04] 查找子串位置
来源：http://ud.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://nz.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://gz.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oc.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://dr.huanxung.cn

Java: s.indexOf("x")
来源：http://hx.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://je.bjjhwx.cn

Ruby: s.index("x")
来源：http://qt.nszjky.cn

C#:   s.IndexOf("x")
来源：http://vb.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lm.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mq.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vq.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ll.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dg.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uf.nicolike.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pi.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qj.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uu.huixiangedu.cn

[E06] 替换子串
来源：http://qv.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ls.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://lf.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fk.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://mf.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vk.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cd.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ad.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://cn.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://ys.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ub.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cw.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bx.shxzskj.cn

TS:   s.split(",")
来源：http://ta.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pu.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://go.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://ug.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iq.asd995.cn

[E08] 数组按分隔符合并
来源：http://dl.panjiajie.cn

Py:   ",".join(items)
来源：http://en.shxzskj.cn

PHP:  implode(",", $items);
来源：http://es.shxzukj.cn

JS:   items.join(",")
来源：http://iu.wgjwhj.cn

TS:   items.join(",")
来源：http://ny.haigaiapp.cn

Java: String.join(",", items)
来源：http://ja.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://jd.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://ix.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://ug.asd995.cn

[E09] 去除所有空白字符
来源：http://zg.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pa.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://iq.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://nc.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://jn.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://ul.jianghongdianzi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hc.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dh.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zd.haigaiapp.cn

[E10] 左侧补零 / 定长填充
来源：http://ls.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xk.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aw.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://ul.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://xo.9csxet.cn

Java: String.format("%03d", 7)
来源：http://nw.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bj.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mx.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xn.jianghongdianzi.cn

[E11] 反转字符串
来源：http://sl.jctech888.com.cn

Py:   s[::-1]
来源：http://nr.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://ax.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://ps.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://jf.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://am.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ug.shtwfgs.cn

Ruby: s.reverse
来源：http://bu.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oa.9csxet.cn

[E12] 统计某字符出现次数
来源：http://oy.bjjhwx.cn

Py:   s.count("a")
来源：http://ju.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://vt.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://rl.521024.cn

TS:   s.split("a").length - 1
来源：http://po.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ln.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://wz.bookmarksfly.cn

Ruby: s.count("a")
来源：http://jj.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://bi.hahajie.cn

[E13] 逐字符遍历
来源：http://bb.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://tu.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ul.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ol.asd995.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fl.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ie.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ok.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lf.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cw.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://ic.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qb.bookmarksfly.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kz.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rj.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qa.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vn.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://id.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eo.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rs.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://jv.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://oh.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://at.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mt.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fb.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yi.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ds.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xj.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ja.nicolike.cn

[E16] 数字千分位
来源：http://ek.nicolike.cn

Py:   f"{1234567:,}"
来源：http://hr.shxzskj.cn

PHP:  number_format(1234567);
来源：http://nj.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ex.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wr.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ku.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qe.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://en.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://fm.huanxung.cn

[E17] 首字母大写
来源：http://ss.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sq.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fu.yuntaijiaju.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hm.yuntaijiaju.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dd.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ne.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yv.huixiangedu.cn

Ruby: s.capitalize
来源：http://tv.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kk.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://nc.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xf.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://et.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mm.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://km.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ra.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oc.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vf.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hi.newstarts.cn

[E19] 多行文本按行拆分
来源：http://fs.bookmarksfly.cn

Py:   s.splitlines()
来源：http://fi.nicolike.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qm.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://kt.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://jw.haigaiapp.cn

Java: s.lines().toList()
来源：http://id.hahajie.cn

Go:   strings.Split(s, "\n")
来源：http://dt.hahajie.cn

Ruby: s.lines
来源：http://kv.nicolike.cn

C#:   s.Split('\n')
来源：http://sh.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://rz.521024.cn

Py:   if not s:
来源：http://ye.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yr.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hh.huanxung.cn

TS:   if (s === "") {}
来源：http://cg.huixiangedu.cn

Java: if (s.isEmpty()) {}
来源：http://sg.huanxung.cn

Go:   if s == "" {}
来源：http://gr.szxytkj.cn

Ruby: if s.empty?
来源：http://ro.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xh.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://js.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ke.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gu.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dq.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ng.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ph.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://ks.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nc.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xz.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://bw.shxzukj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vi.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fj.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gs.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nc.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kd.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://em.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://rf.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wh.yuntaijiaju.cn

================================================================================
来源：http://lh.nszjky.cn

F. 文件与目录
来源：http://sz.chemitech.net.cn

================================================================================
来源：http://ix.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://zd.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xq.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://gf.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zd.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rr.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://it.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zs.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://jm.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://vg.bjjhwx.cn

[F02] 逐行读取文件
来源：http://sk.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gx.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qh.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eg.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wg.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qc.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kh.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kc.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nd.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://mt.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cp.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bu.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tl.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ub.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jg.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dt.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://om.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://un.shtwfgs.cn

[F04] 追加写入文件
来源：http://ju.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://be.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bo.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://va.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sn.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pf.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pe.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ok.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uu.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://by.shxzskj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ka.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://ei.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://rq.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://hf.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tj.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ra.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://nv.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://cu.hnjuh.cn

[F06] 删除文件
来源：http://eb.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://al.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://lu.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fc.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yf.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jd.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://ml.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://el.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://en.colortex.cn

[F07] 创建目录（含多级）
来源：http://wn.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tq.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mz.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ti.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bt.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tx.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bd.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lm.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://og.newstarts.cn

[F08] 遍历目录
来源：http://dj.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sg.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zq.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://mg.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://yc.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://og.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qg.nszjky.cn

Ruby: Dir.children("dir")
来源：http://kv.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://pp.panjiajie.cn

[F09] 获取文件大小
来源：http://th.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://rr.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://xy.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://kr.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://as.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fi.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gp.newstarts.cn

Ruby: File.size("a.txt")
来源：http://ef.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://dg.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://ho.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wv.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gr.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jy.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://cp.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nd.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fg.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lt.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sa.lnxyls.cn

[F11] 复制与移动文件
来源：http://ks.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rs.newstarts.cn


<!-- 参考信息 -->