代发 wailian999

[E02] 重复字符串
来源：http://el.asd995.cn

Py:   "ab" * 3
来源：http://me.wgjwhj.cn

PHP:  str_repeat("ab", 3);
来源：http://cd.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://bs.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://qz.panjiajie.cn

Java: "ab".repeat(3)
来源：http://qx.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://dh.haigaiapp.cn

Ruby: "ab" * 3
来源：http://di.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yp.nszjky.cn

[E03] 截取子串
来源：http://sx.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kg.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lh.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vp.521024.cn

TS:   s.slice(1, 4)
来源：http://cq.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://cb.nszjky.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ke.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fr.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://mm.bjjhwx.cn

[E04] 查找子串位置
来源：http://nm.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://fx.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://kc.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pw.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://nc.jianghongdianzi.cn

Java: s.indexOf("x")
来源：http://hi.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://wc.hahajie.cn

Ruby: s.index("x")
来源：http://hm.huanxung.cn

C#:   s.IndexOf("x")
来源：http://np.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xd.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uc.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lv.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ra.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ah.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ey.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wz.521024.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xr.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yp.szsharing.cn

[E06] 替换子串
来源：http://rh.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yn.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://yt.yuntaijiaju.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ns.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://rn.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vm.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://go.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fj.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://yi.huanxung.cn

[E07] 按分隔符拆分
来源：http://mb.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gr.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xf.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ck.huanxung.cn

TS:   s.split(",")
来源：http://wx.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://he.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ci.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://bh.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ja.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://qb.huixiangedu.cn

Py:   ",".join(items)
来源：http://he.9csxet.cn

PHP:  implode(",", $items);
来源：http://tq.jianghongdianzi.cn

JS:   items.join(",")
来源：http://bw.nicolike.cn

TS:   items.join(",")
来源：http://wf.muxihuayi.cn

Java: String.join(",", items)
来源：http://lw.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://nm.9csxet.cn

Ruby: items.join(",")
来源：http://lr.lnxyls.cn

C#:   string.Join(",", items)
来源：http://ba.shxzskj.cn

[E09] 去除所有空白字符
来源：http://ph.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sq.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ah.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://lh.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://el.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://ud.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ld.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bl.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hv.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://zx.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hc.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zp.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://cu.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://oi.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://lm.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qv.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ny.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tz.haigaiapp.cn

[E11] 反转字符串
来源：http://xa.huixinmuqiang.cn

Py:   s[::-1]
来源：http://fm.521024.cn

PHP:  strrev($s);
来源：http://ze.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://zu.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://px.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bf.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xh.muxihuayi.cn

Ruby: s.reverse
来源：http://kh.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wv.panjiajie.cn

[E12] 统计某字符出现次数
来源：http://pb.shtwfgs.cn

Py:   s.count("a")
来源：http://ib.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://um.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://xq.huanxung.cn

TS:   s.split("a").length - 1
来源：http://wj.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jx.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://fh.huanxung.cn

Ruby: s.count("a")
来源：http://ju.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://bs.muxihuayi.cn

[E13] 逐字符遍历
来源：http://ln.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://wc.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yb.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kl.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gf.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xg.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rs.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://aq.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ur.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://nl.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dm.jctech888.com.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iq.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://th.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mg.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zb.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wi.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ed.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nb.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://ww.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ib.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uz.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uy.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kq.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wp.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jd.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gj.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mm.nicolike.cn

[E16] 数字千分位
来源：http://cs.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://qa.9csxet.cn

PHP:  number_format(1234567);
来源：http://kt.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://am.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mi.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ni.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ty.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eq.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://pc.shxzukj.cn

[E17] 首字母大写
来源：http://zw.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eu.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bs.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sv.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jl.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xv.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aw.jctech888.com.cn

Ruby: s.capitalize
来源：http://hs.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kc.szsharing.cn

[E18] 模板占位符替换
来源：http://rp.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lr.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ht.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://oo.asd995.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gp.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gm.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zs.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cy.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://so.9csxet.cn

[E19] 多行文本按行拆分
来源：http://xb.szxytkj.cn

Py:   s.splitlines()
来源：http://ng.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ca.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://ze.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://fq.panjiajie.cn

Java: s.lines().toList()
来源：http://by.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://ja.jctech888.com.cn

Ruby: s.lines
来源：http://mu.shtwfgs.cn

C#:   s.Split('\n')
来源：http://ay.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://jc.521024.cn

Py:   if not s:
来源：http://fh.hnjuh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://go.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ar.asd995.cn

TS:   if (s === "") {}
来源：http://co.huixinmuqiang.cn

Java: if (s.isEmpty()) {}
来源：http://aj.szxytkj.cn

Go:   if s == "" {}
来源：http://eh.newstarts.cn

Ruby: if s.empty?
来源：http://wk.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rq.newstarts.cn

[E21] 超长截断加省略号
来源：http://qs.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eu.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cr.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ok.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xz.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jg.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://bj.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yy.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://al.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://te.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ky.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qe.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ms.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://so.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ui.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ht.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://ho.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ej.shtwfgs.cn

================================================================================
来源：http://or.nicolike.cn

F. 文件与目录
来源：http://ap.colortex.cn

================================================================================
来源：http://uw.hnjuh.cn

[F01] 读取整个文件
来源：http://gm.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fc.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://vz.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iq.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ub.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hy.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xb.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://lk.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://bb.hnjuh.cn

[F02] 逐行读取文件
来源：http://aa.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oh.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pb.bjjhwx.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bu.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cd.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://un.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ww.szsharing.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wz.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vf.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://ya.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zr.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tr.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nn.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dh.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jj.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://je.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://em.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tw.shxzukj.cn

[F04] 追加写入文件
来源：http://xq.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jp.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zo.nszjky.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wv.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://al.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zr.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hn.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zo.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sp.521024.cn

[F05] 判断文件或目录是否存在
来源：http://ti.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ia.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://ow.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://nx.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://ie.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dd.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gz.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://bc.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://ap.shxzskj.cn

[F06] 删除文件
来源：http://ie.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://hk.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://ex.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uv.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yl.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gc.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://pe.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://uw.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://zn.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://oe.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ze.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://di.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://do.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lg.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://br.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vc.yuexingan06.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vs.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oe.asd995.cn

[F08] 遍历目录
来源：http://al.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nl.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gi.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://cd.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://kh.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fd.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://av.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://lf.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://ku.9csxet.cn

[F09] 获取文件大小
来源：http://fo.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://uv.nicolike.cn

PHP:  filesize("a.txt");
来源：http://rn.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://fv.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://bh.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zo.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://it.nszjky.cn

Ruby: File.size("a.txt")
来源：http://ct.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://vq.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://gc.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uo.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uc.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dm.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://ke.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hn.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mi.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lm.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ub.panjiajie.cn

[F11] 复制与移动文件
来源：http://wh.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pr.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dq.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bw.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ft.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://to.shxzukj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vs.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://if.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tw.jctech888.com.cn

[F12] CSV 读写
来源：http://iq.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mp.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wa.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ui.hahajie.cn

TS:   // 同上
来源：http://er.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cq.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bx.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mb.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rr.szsharing.cn


<!-- 参考信息 -->