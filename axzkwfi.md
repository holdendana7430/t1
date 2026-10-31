代发 wailian999

[E02] 重复字符串
来源：http://rk.huixiangedu.cn

Py:   "ab" * 3
来源：http://aa.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://ji.nszjky.cn

JS:   "ab".repeat(3)
来源：http://wc.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://ju.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://mp.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://rx.9csxet.cn

Ruby: "ab" * 3
来源：http://lv.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ap.gzmigu.cn

[E03] 截取子串
来源：http://kp.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cb.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jt.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rj.newstarts.cn

TS:   s.slice(1, 4)
来源：http://ul.nicolike.cn

Java: s.substring(1, 4)
来源：http://iq.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kb.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zb.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://oc.shxzukj.cn

[E04] 查找子串位置
来源：http://fs.asd995.cn

Py:   s.find("x");  s.index("x")
来源：http://ac.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://yi.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://st.hahajie.cn

TS:   s.indexOf("x")
来源：http://wb.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://xb.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://fr.panjiajie.cn

Ruby: s.index("x")
来源：http://qz.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://ar.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bc.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://go.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ne.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ij.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fb.wgjwhj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kq.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ug.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://za.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wx.lnxyls.cn

[E06] 替换子串
来源：http://le.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yz.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://ix.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lb.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://dg.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bf.yuntaijiaju.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aa.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lc.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://tq.szxytkj.cn

[E07] 按分隔符拆分
来源：http://je.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wg.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://za.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qv.huixinmuqiang.cn

TS:   s.split(",")
来源：http://jw.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ws.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ix.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://jc.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pk.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://dw.shxzukj.cn

Py:   ",".join(items)
来源：http://ie.hnjuh.cn

PHP:  implode(",", $items);
来源：http://gz.shxzukj.cn

JS:   items.join(",")
来源：http://qf.shxzukj.cn

TS:   items.join(",")
来源：http://em.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://zq.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://fy.yuexingan06.cn

Ruby: items.join(",")
来源：http://cs.lnxyls.cn

C#:   string.Join(",", items)
来源：http://oj.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://zh.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eb.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ve.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://pe.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://th.nszjky.cn

Java: s.replaceAll("\\s+", "")
来源：http://to.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://th.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rj.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fq.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://pa.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ka.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dg.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://qv.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://mr.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://tn.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gm.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kb.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://em.colortex.cn

[E11] 反转字符串
来源：http://gl.nszjky.cn

Py:   s[::-1]
来源：http://an.nicolike.cn

PHP:  strrev($s);
来源：http://mp.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://rr.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://fr.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vo.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bz.muxihuayi.cn

Ruby: s.reverse
来源：http://pq.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://md.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://lu.huixinmuqiang.cn

Py:   s.count("a")
来源：http://cg.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://ar.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://ko.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://go.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ng.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://yp.lnxyls.cn

Ruby: s.count("a")
来源：http://vp.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://hi.panjiajie.cn

[E13] 逐字符遍历
来源：http://lj.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://bp.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kd.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hu.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nz.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kr.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lx.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zh.bookmarksfly.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bk.muxihuayi.cn

[E14] URL 编码与 Base64
来源：http://qe.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sr.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jd.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mm.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ou.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fq.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ak.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://er.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yu.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://qf.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jt.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wv.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pv.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://an.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rp.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hs.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xs.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wx.shtwfgs.cn

[E16] 数字千分位
来源：http://nj.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://dp.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://gf.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xj.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tg.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ef.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yi.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rf.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://ht.shtwfgs.cn

[E17] 首字母大写
来源：http://dp.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tm.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vv.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ew.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fp.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ea.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dn.bjjhwx.cn

Ruby: s.capitalize
来源：http://io.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cz.colortex.cn

[E18] 模板占位符替换
来源：http://in.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zo.gzmigu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ik.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pc.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fz.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lf.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ep.hnjuh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gb.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://at.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://sp.muxihuayi.cn

Py:   s.splitlines()
来源：http://io.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jx.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://qa.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://so.shxzskj.cn

Java: s.lines().toList()
来源：http://mr.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://zy.huixinmuqiang.cn

Ruby: s.lines
来源：http://qz.shtwfgs.cn

C#:   s.Split('\n')
来源：http://eo.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://yr.521024.cn

Py:   if not s:
来源：http://kq.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cl.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bo.huanxung.cn

TS:   if (s === "") {}
来源：http://dd.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://rm.yuexingan06.cn

Go:   if s == "" {}
来源：http://gg.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://gp.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nl.colortex.cn

[E21] 超长截断加省略号
来源：http://ja.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bm.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iq.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mu.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ty.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ab.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://zh.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mr.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pn.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://nb.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bx.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ay.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qb.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ez.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kx.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gs.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://eh.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jr.shtwfgs.cn

================================================================================
来源：http://fv.huanxung.cn

F. 文件与目录
来源：http://xw.shxzukj.cn

================================================================================
来源：http://nx.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://kj.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jw.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://mu.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cf.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mf.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pv.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ru.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://uu.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://gs.asd995.cn

[F02] 逐行读取文件
来源：http://im.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://om.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rt.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gt.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ai.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ev.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pq.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qf.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ig.521024.cn

[F03] 写入文件（覆盖）
来源：http://bj.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aq.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lh.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://av.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ak.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xy.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uj.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://vr.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zu.huanxung.cn

[F04] 追加写入文件
来源：http://gm.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mo.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://va.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tj.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://se.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://em.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vr.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lb.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kx.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://et.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ve.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://lz.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://ua.lnxyls.cn

TS:   fs.existsSync("a.txt")
来源：http://ty.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ph.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ql.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://xx.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://pl.wgjwhj.cn

[F06] 删除文件
来源：http://jf.nszjky.cn

Py:   os.remove("a.txt")
来源：http://ah.asd995.cn

PHP:  unlink("a.txt");
来源：http://gi.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dh.szxytkj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wj.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pn.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://qb.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://av.521024.cn

C#:   File.Delete("a.txt");
来源：http://dv.newstarts.cn

[F07] 创建目录（含多级）
来源：http://dn.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fj.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fm.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aq.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pc.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://el.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hr.yuexingan06.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kb.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vu.shtwfgs.cn

[F08] 遍历目录
来源：http://yw.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tj.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nl.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://mf.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://cq.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mz.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yz.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://gn.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://cj.9csxet.cn

[F09] 获取文件大小
来源：http://pl.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://kp.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://gh.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://mp.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://pt.9csxet.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gj.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gl.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://md.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://le.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://nb.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zp.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ik.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bi.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://sm.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yn.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wx.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aa.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qm.nicolike.cn

[F11] 复制与移动文件
来源：http://vl.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ng.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tc.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://op.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fb.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cw.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jm.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bs.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yc.nicolike.cn

[F12] CSV 读写
来源：http://cv.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://de.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ia.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iy.chemitech.net.cn

TS:   // 同上
来源：http://wf.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hh.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fx.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xt.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rd.hnjuh.cn


<!-- 参考信息 -->