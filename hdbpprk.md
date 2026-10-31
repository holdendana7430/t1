代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jt.colortex.cn

[E03] 截取子串
来源：http://zs.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yk.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bi.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zu.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://bq.colortex.cn

Java: s.substring(1, 4)
来源：http://cj.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ms.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jw.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://mh.szsharing.cn

[E04] 查找子串位置
来源：http://ba.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://ub.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://tq.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yw.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://gx.jctech888.com.cn

Java: s.indexOf("x")
来源：http://ib.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://vs.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://nm.colortex.cn

C#:   s.IndexOf("x")
来源：http://wv.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gm.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cr.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qz.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ob.shxzskj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xj.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hi.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vs.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iu.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bi.asd995.cn

[E06] 替换子串
来源：http://yj.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ke.huanxung.cn

PHP:  str_replace("a", "b", $s);
来源：http://lq.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mw.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://cy.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nr.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ir.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dg.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://rj.nszjky.cn

[E07] 按分隔符拆分
来源：http://el.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ig.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://na.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ke.muxihuayi.cn

TS:   s.split(",")
来源：http://pk.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vd.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kc.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://ef.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dw.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://sv.shtwfgs.cn

Py:   ",".join(items)
来源：http://uu.hnjuh.cn

PHP:  implode(",", $items);
来源：http://rw.lnxyls.cn

JS:   items.join(",")
来源：http://hm.colortex.cn

TS:   items.join(",")
来源：http://vx.panjiajie.cn

Java: String.join(",", items)
来源：http://ka.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://pq.huanxung.cn

Ruby: items.join(",")
来源：http://hi.szsharing.cn

C#:   string.Join(",", items)
来源：http://cs.hnjuh.cn

[E09] 去除所有空白字符
来源：http://jb.colortex.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mk.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bo.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://bf.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://dd.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://pj.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qt.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pw.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nn.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://cx.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cy.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://it.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://kw.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://lz.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://vp.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://md.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wl.yuexingan06.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gh.nicolike.cn

[E11] 反转字符串
来源：http://yf.521024.cn

Py:   s[::-1]
来源：http://vj.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://vo.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://jm.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://dg.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://is.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yx.colortex.cn

Ruby: s.reverse
来源：http://gd.nszjky.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zg.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://yp.asd995.cn

Py:   s.count("a")
来源：http://ti.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://vv.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://xv.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://ev.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qt.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://fu.gzmigu.cn

Ruby: s.count("a")
来源：http://bk.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://hn.muxihuayi.cn

[E13] 逐字符遍历
来源：http://aj.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://rc.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fq.bjjhwx.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tq.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jc.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qr.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rw.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bf.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://im.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://gm.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ba.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://in.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hr.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xg.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://om.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kz.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://la.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xe.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://oe.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zl.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oc.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ho.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wz.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ua.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wq.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qi.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yo.shxzukj.cn

[E16] 数字千分位
来源：http://bb.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://go.szxytkj.cn

PHP:  number_format(1234567);
来源：http://ty.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tj.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kq.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tn.gzmigu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bm.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hu.yuexingan06.cn

C#:   1234567.ToString("N0")
来源：http://hx.szsharing.cn

[E17] 首字母大写
来源：http://zd.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cm.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sm.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ao.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hd.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vg.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fl.shxzukj.cn

Ruby: s.capitalize
来源：http://tg.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yn.szsharing.cn

[E18] 模板占位符替换
来源：http://om.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wp.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://su.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dh.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ea.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://en.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://la.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fe.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jp.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://lj.huixiangedu.cn

Py:   s.splitlines()
来源：http://yy.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qu.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://mq.huixiangedu.cn

TS:   s.split(/\r?\n/)
来源：http://qw.9csxet.cn

Java: s.lines().toList()
来源：http://fk.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://yy.newstarts.cn

Ruby: s.lines
来源：http://bg.haigaiapp.cn

C#:   s.Split('\n')
来源：http://qa.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://rh.bjjhwx.cn

Py:   if not s:
来源：http://mw.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bv.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fg.huixiangedu.cn

TS:   if (s === "") {}
来源：http://pg.huixinmuqiang.cn

Java: if (s.isEmpty()) {}
来源：http://mb.panjiajie.cn

Go:   if s == "" {}
来源：http://qg.szxytkj.cn

Ruby: if s.empty?
来源：http://cu.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wk.colortex.cn

[E21] 超长截断加省略号
来源：http://mo.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aw.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://un.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jb.chemitech.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rg.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ki.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://tp.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://er.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ms.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://zw.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ah.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aa.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gu.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vz.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://or.521024.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pb.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://ff.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oy.colortex.cn

================================================================================
来源：http://vn.gzmigu.cn

F. 文件与目录
来源：http://vf.colortex.cn

================================================================================
来源：http://zk.9csxet.cn

[F01] 读取整个文件
来源：http://dn.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xm.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://rc.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xa.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lf.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ja.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xy.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://xs.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://np.wgjwhj.cn

[F02] 逐行读取文件
来源：http://hp.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kr.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bz.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jh.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vk.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ly.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nf.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ks.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gq.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://lz.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ap.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://aj.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://my.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://id.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ad.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tj.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://qj.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tp.chemitech.net.cn

[F04] 追加写入文件
来源：http://cm.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://we.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jb.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fs.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mr.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gh.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rv.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://py.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yr.colortex.cn

[F05] 判断文件或目录是否存在
来源：http://ah.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mr.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://af.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://bi.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://fn.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yu.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fw.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://go.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://tk.bookmarksfly.cn

[F06] 删除文件
来源：http://xz.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://zl.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://bp.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://io.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ix.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pp.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://ha.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://ag.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://jd.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://dd.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vb.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qp.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uw.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xw.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ay.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dx.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://be.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qa.newstarts.cn

[F08] 遍历目录
来源：http://ea.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yl.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://py.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://lp.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://oh.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gq.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zt.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://qp.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://xh.yuexingan06.cn

[F09] 获取文件大小
来源：http://lb.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://xc.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://wm.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://kh.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://rl.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kc.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://de.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://pn.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://rl.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://er.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ea.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ul.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vn.521024.cn

TS:   path.extname("a.txt")
来源：http://qv.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://er.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lv.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wv.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yx.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://gr.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cn.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lg.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gq.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rg.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vk.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://px.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ea.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xe.jianghongdianzi.cn

[F12] CSV 读写
来源：http://ps.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qz.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lu.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lo.wgjwhj.cn

TS:   // 同上
来源：http://sp.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qp.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ct.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yn.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hi.wgjwhj.cn

================================================================================
来源：http://co.colortex.cn

G. 面向对象
来源：http://ki.bookmarksfly.cn

================================================================================
来源：http://tp.521024.cn

[G01] 定义类
来源：http://ql.nszjky.cn

Py:   class User: pass
来源：http://wf.huixinmuqiang.cn

PHP:  class User {}
来源：http://bw.jianghongdianzi.cn

JS:   class User {}
来源：http://ad.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://cb.shxzskj.cn


<!-- 参考信息 -->