代发 wailian999

[E02] 重复字符串
来源：http://cz.newstarts.cn

Py:   "ab" * 3
来源：http://iv.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://oq.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://cb.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://xp.shxzukj.cn

Java: "ab".repeat(3)
来源：http://lt.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://cz.yuexingan06.cn

Ruby: "ab" * 3
来源：http://lw.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rk.shxzskj.cn

[E03] 截取子串
来源：http://ec.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xc.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://px.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yc.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://qw.asd995.cn

Java: s.substring(1, 4)
来源：http://gj.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fs.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://eo.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://dh.wgjwhj.cn

[E04] 查找子串位置
来源：http://vj.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://bp.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://rq.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ba.newstarts.cn

TS:   s.indexOf("x")
来源：http://lq.panjiajie.cn

Java: s.indexOf("x")
来源：http://an.521024.cn

Go:   strings.Index(s, "x")
来源：http://sl.bjjhwx.cn

Ruby: s.index("x")
来源：http://ib.nszjky.cn

C#:   s.IndexOf("x")
来源：http://qh.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zl.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ug.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pq.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wx.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uz.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oq.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sj.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gx.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pq.wgjwhj.cn

[E06] 替换子串
来源：http://cn.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qa.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://xc.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ua.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://lv.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eq.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ki.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ze.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://zs.hahajie.cn

[E07] 按分隔符拆分
来源：http://ei.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ho.szsharing.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qo.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://td.wgjwhj.cn

TS:   s.split(",")
来源：http://hz.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vp.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dd.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://bs.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uu.nszjky.cn

[E08] 数组按分隔符合并
来源：http://rb.colortex.cn

Py:   ",".join(items)
来源：http://vx.shxzskj.cn

PHP:  implode(",", $items);
来源：http://ie.haigaiapp.cn

JS:   items.join(",")
来源：http://ji.yuexingan06.cn

TS:   items.join(",")
来源：http://eu.colortex.cn

Java: String.join(",", items)
来源：http://px.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://ek.haigaiapp.cn

Ruby: items.join(",")
来源：http://ri.panjiajie.cn

C#:   string.Join(",", items)
来源：http://ku.521024.cn

[E09] 去除所有空白字符
来源：http://ge.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gf.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ek.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://do.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://bj.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://pu.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sw.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yz.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gr.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://jf.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ey.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gt.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://wv.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://an.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://yi.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xh.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://id.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nu.huixinmuqiang.cn

[E11] 反转字符串
来源：http://ue.haigaiapp.cn

Py:   s[::-1]
来源：http://ug.huanxung.cn

PHP:  strrev($s);
来源：http://qo.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://zp.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://mm.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lf.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sy.bookmarksfly.cn

Ruby: s.reverse
来源：http://lz.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sn.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://yf.shxzskj.cn

Py:   s.count("a")
来源：http://no.yuexingan06.cn

PHP:  substr_count($s, "a");
来源：http://qf.huanxung.cn

JS:   s.split("a").length - 1
来源：http://fo.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://ef.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zf.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://om.bookmarksfly.cn

Ruby: s.count("a")
来源：http://wr.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://jc.shxzukj.cn

[E13] 逐字符遍历
来源：http://ee.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://gb.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oz.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ff.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://oj.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bq.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dz.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mm.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kq.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://de.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://um.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://af.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jx.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lb.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nt.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fu.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pz.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://su.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://wg.colortex.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lw.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://js.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ce.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mp.huanxung.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ch.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zq.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nn.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ex.huixinmuqiang.cn

[E16] 数字千分位
来源：http://af.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://pv.shxzskj.cn

PHP:  number_format(1234567);
来源：http://dq.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dh.asd995.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mh.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qe.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hc.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nh.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://fp.yuntaijiaju.cn

[E17] 首字母大写
来源：http://ut.shxzskj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pj.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://av.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://of.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ak.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://at.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://le.huixiangedu.cn

Ruby: s.capitalize
来源：http://no.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iw.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://cd.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tl.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bs.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wl.gzmigu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xf.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lm.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ak.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://km.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ao.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://in.haigaiapp.cn

Py:   s.splitlines()
来源：http://ni.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ka.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://cc.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://dr.9csxet.cn

Java: s.lines().toList()
来源：http://ol.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://an.haigaiapp.cn

Ruby: s.lines
来源：http://xc.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://wg.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://ku.wgjwhj.cn

Py:   if not s:
来源：http://qu.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ui.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rb.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://av.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://rw.szsharing.cn

Go:   if s == "" {}
来源：http://mu.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://hw.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xo.shxzskj.cn

[E21] 超长截断加省略号
来源：http://zr.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://op.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zt.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sv.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://td.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ah.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://sh.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oh.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sj.521024.cn

[E22] 字节长度与字符长度
来源：http://js.hnjuh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ii.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jc.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ht.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gx.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xg.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ch.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://gt.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sg.wgjwhj.cn

================================================================================
来源：http://dg.colortex.cn

F. 文件与目录
来源：http://vj.huanxung.cn

================================================================================
来源：http://ds.wgjwhj.cn

[F01] 读取整个文件
来源：http://es.chemitech.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iu.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://en.hnjuh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tm.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hv.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qk.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vt.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://uv.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://sz.bjjhwx.cn

[F02] 逐行读取文件
来源：http://bp.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cl.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gl.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wj.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zi.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zx.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dh.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bu.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mz.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://du.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pz.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ku.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ip.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gp.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nd.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gn.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://vu.yuntaijiaju.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gq.shxzskj.cn

[F04] 追加写入文件
来源：http://cn.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pi.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yl.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ir.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://an.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rc.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vb.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nk.shxzukj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ng.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://ne.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nl.colortex.cn

PHP:  file_exists("a.txt");
来源：http://ls.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://tp.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://aj.shxzskj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oz.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ap.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://hk.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://mu.9csxet.cn

[F06] 删除文件
来源：http://aa.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://fd.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://au.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pj.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nz.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yt.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://ch.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://dy.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://ox.nicolike.cn

[F07] 创建目录（含多级）
来源：http://td.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wq.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qq.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://au.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nc.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ou.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ln.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gj.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ke.shxzskj.cn

[F08] 遍历目录
来源：http://ci.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zx.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pb.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://cg.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://uy.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jw.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pv.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://rl.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://zp.muxihuayi.cn

[F09] 获取文件大小
来源：http://pt.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://ps.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://oh.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://lc.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://un.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dj.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mp.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://dw.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://ef.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://tt.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hv.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ht.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rj.nicolike.cn

TS:   path.extname("a.txt")
来源：http://cw.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dg.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nu.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://he.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cv.hahajie.cn

[F11] 复制与移动文件
来源：http://rk.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bo.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tf.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://py.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wk.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nt.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fl.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sk.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xh.yuexingan06.cn

[F12] CSV 读写
来源：http://ne.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wm.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gx.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dl.asd995.cn

TS:   // 同上
来源：http://kx.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lb.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qt.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jl.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kv.szxytkj.cn


<!-- 参考信息 -->