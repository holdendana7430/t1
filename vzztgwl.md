代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jv.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://ve.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://tg.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tj.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ew.colortex.cn

C#:   s.Substring(1, 3)
来源：http://mt.shtwfgs.cn

[E04] 查找子串位置
来源：http://mu.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://dg.hahajie.cn

PHP:  strpos($s, "x");
来源：http://gy.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fs.gzmigu.cn

TS:   s.indexOf("x")
来源：http://yz.huanxung.cn

Java: s.indexOf("x")
来源：http://br.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://ex.bjjhwx.cn

Ruby: s.index("x")
来源：http://dv.huanxung.cn

C#:   s.IndexOf("x")
来源：http://qu.huanxung.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bm.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nq.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cy.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dw.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fd.lnxyls.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oj.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://im.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fu.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://do.newstarts.cn

[E06] 替换子串
来源：http://om.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yw.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://sf.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lg.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://av.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oj.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jd.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iy.jctech888.com.cn

C#:   s.Replace("a", "b")
来源：http://ks.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://os.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pz.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zz.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xu.panjiajie.cn

TS:   s.split(",")
来源：http://ai.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tz.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vv.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://uq.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cc.asd995.cn

[E08] 数组按分隔符合并
来源：http://vv.nszjky.cn

Py:   ",".join(items)
来源：http://bs.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://wa.lnxyls.cn

JS:   items.join(",")
来源：http://yq.chemitech.net.cn

TS:   items.join(",")
来源：http://ba.nszjky.cn

Java: String.join(",", items)
来源：http://ud.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://xw.hnjuh.cn

Ruby: items.join(",")
来源：http://sc.colortex.cn

C#:   string.Join(",", items)
来源：http://cr.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://pg.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mf.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dj.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://zj.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://vm.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ec.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wq.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sv.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rx.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://bv.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ce.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jx.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://kj.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://na.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://pi.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ky.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ai.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kj.muxihuayi.cn

[E11] 反转字符串
来源：http://ug.lnxyls.cn

Py:   s[::-1]
来源：http://ut.hahajie.cn

PHP:  strrev($s);
来源：http://pr.asd995.cn

JS:   [...s].reverse().join("")
来源：http://jt.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://xq.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://el.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qh.jctech888.com.cn

Ruby: s.reverse
来源：http://gn.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tb.colortex.cn

[E12] 统计某字符出现次数
来源：http://fa.chemitech.net.cn

Py:   s.count("a")
来源：http://vo.szxytkj.cn

PHP:  substr_count($s, "a");
来源：http://zw.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://my.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://ux.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nj.asd995.cn

Go:   strings.Count(s, "a")
来源：http://su.colortex.cn

Ruby: s.count("a")
来源：http://gv.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://yx.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://oo.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://fm.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mr.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://as.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ae.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ar.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ss.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://iq.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ci.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://eo.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://et.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wm.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gd.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gq.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ou.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ek.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://du.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://as.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://ii.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ar.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qs.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oe.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ug.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://me.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://js.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hi.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nw.wgjwhj.cn

[E16] 数字千分位
来源：http://vj.nszjky.cn

Py:   f"{1234567:,}"
来源：http://sz.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://my.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sz.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://un.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uz.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zc.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xy.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://ch.bjjhwx.cn

[E17] 首字母大写
来源：http://nd.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nr.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://an.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kn.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zv.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kb.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jz.szsharing.cn

Ruby: s.capitalize
来源：http://vb.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ku.gzmigu.cn

[E18] 模板占位符替换
来源：http://xx.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qc.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pb.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fq.lnxyls.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bi.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pn.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wu.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bv.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jj.9csxet.cn

[E19] 多行文本按行拆分
来源：http://om.nszjky.cn

Py:   s.splitlines()
来源：http://tn.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jf.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://rl.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://mn.nszjky.cn

Java: s.lines().toList()
来源：http://eg.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://ys.jctech888.com.cn

Ruby: s.lines
来源：http://pz.521024.cn

C#:   s.Split('\n')
来源：http://cu.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://rg.huanxung.cn

Py:   if not s:
来源：http://tr.chemitech.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hn.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eg.huanxung.cn

TS:   if (s === "") {}
来源：http://wr.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://bm.hnjuh.cn

Go:   if s == "" {}
来源：http://aq.gzmigu.cn

Ruby: if s.empty?
来源：http://up.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fw.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://tz.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cs.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fg.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ex.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://td.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mz.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://sl.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kn.asd995.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ws.nszjky.cn

[E22] 字节长度与字符长度
来源：http://el.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://op.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dl.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ca.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ft.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qn.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xm.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://jh.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vz.bookmarksfly.cn

================================================================================
来源：http://wf.nicolike.cn

F. 文件与目录
来源：http://mn.521024.cn

================================================================================
来源：http://py.jctech888.com.cn

[F01] 读取整个文件
来源：http://nu.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gm.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://xe.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ea.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yj.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dg.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jp.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://uj.asd995.cn

C#:   File.ReadAllText("a.txt");
来源：http://xy.9csxet.cn

[F02] 逐行读取文件
来源：http://ya.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dc.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ob.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lt.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yk.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://em.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hi.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yf.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zj.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://ea.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zj.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hj.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sg.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mz.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kl.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ln.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://pu.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kw.chemitech.net.cn

[F04] 追加写入文件
来源：http://ke.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gm.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://si.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ay.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ka.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jo.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nl.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kf.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://us.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://vn.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bf.colortex.cn

PHP:  file_exists("a.txt");
来源：http://ho.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://sf.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://yu.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tr.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ho.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://bk.colortex.cn

C#:   File.Exists("a.txt")
来源：http://ov.wgjwhj.cn

[F06] 删除文件
来源：http://hf.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://rd.colortex.cn

PHP:  unlink("a.txt");
来源：http://xd.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ot.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://em.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ia.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://so.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://jn.asd995.cn

C#:   File.Delete("a.txt");
来源：http://kw.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://ik.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tc.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rn.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zj.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ex.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://df.521024.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hc.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wh.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://at.colortex.cn

[F08] 遍历目录
来源：http://zb.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://br.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cj.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://sn.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://mc.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uf.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vc.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://hu.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://kq.asd995.cn

[F09] 获取文件大小
来源：http://hw.haigaiapp.cn

Py:   os.path.getsize("a.txt")
来源：http://mm.asd995.cn

PHP:  filesize("a.txt");
来源：http://ec.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://ei.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://ro.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dd.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nb.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://ee.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://sk.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://io.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wr.haigaiapp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ck.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hv.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://ct.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zn.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://do.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kj.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fi.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://ku.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ck.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fr.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yi.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ke.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tk.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ib.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ia.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://va.nszjky.cn

[F12] CSV 读写
来源：http://dx.colortex.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cu.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://li.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ir.shxzukj.cn

TS:   // 同上
来源：http://bo.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hl.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bc.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nc.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uz.shxzskj.cn

================================================================================
来源：http://mc.newstarts.cn

G. 面向对象
来源：http://dq.521024.cn

================================================================================
来源：http://sw.bjjhwx.cn

[G01] 定义类
来源：http://xt.szxytkj.cn

Py:   class User: pass
来源：http://nb.bjjhwx.cn

PHP:  class User {}
来源：http://ft.shxzukj.cn

JS:   class User {}
来源：http://ez.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://pj.yuexingan06.cn

Java: class User {}
来源：http://kk.newstarts.cn

Go:   type User struct { Name string }
来源：http://jr.jianghongdianzi.cn

Ruby: class User; end
来源：http://vc.asd995.cn

C#:   class User {}
来源：http://et.chemitech.net.cn


<!-- 参考信息 -->