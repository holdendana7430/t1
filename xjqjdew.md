代发 wailian999

Go:   strings.Index(s, "x")
来源：http://mq.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://zg.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://gr.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://se.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ls.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ai.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://as.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ai.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://on.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cb.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sz.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kr.huixiangedu.cn

[E06] 替换子串
来源：http://wh.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rj.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://fw.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zu.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://yo.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xx.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gr.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ij.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://lt.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://jm.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wd.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fh.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vl.muxihuayi.cn

TS:   s.split(",")
来源：http://dx.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nn.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ug.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://gh.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qi.nszjky.cn

[E08] 数组按分隔符合并
来源：http://ii.lnxyls.cn

Py:   ",".join(items)
来源：http://ys.panjiajie.cn

PHP:  implode(",", $items);
来源：http://td.shxzskj.cn

JS:   items.join(",")
来源：http://tp.bjjhwx.cn

TS:   items.join(",")
来源：http://qo.nszjky.cn

Java: String.join(",", items)
来源：http://ol.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://zh.bookmarksfly.cn

Ruby: items.join(",")
来源：http://em.szxytkj.cn

C#:   string.Join(",", items)
来源：http://cb.newstarts.cn

[E09] 去除所有空白字符
来源：http://pv.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qv.huixinmuqiang.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://al.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://mm.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://qk.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://we.gzmigu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cn.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xi.szsharing.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jo.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://fl.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bd.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ea.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://il.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://ls.nicolike.cn

Java: String.format("%03d", 7)
来源：http://bd.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://op.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ap.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xk.newstarts.cn

[E11] 反转字符串
来源：http://vb.bjjhwx.cn

Py:   s[::-1]
来源：http://ul.muxihuayi.cn

PHP:  strrev($s);
来源：http://lf.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://eq.newstarts.cn

TS:   [...s].reverse().join("")
来源：http://sc.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ku.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qe.lnxyls.cn

Ruby: s.reverse
来源：http://bk.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ez.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://kv.9csxet.cn

Py:   s.count("a")
来源：http://wd.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://ns.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://zi.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://ep.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cj.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://ge.shxzukj.cn

Ruby: s.count("a")
来源：http://mc.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://cv.521024.cn

[E13] 逐字符遍历
来源：http://wv.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://bj.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vg.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dn.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://iw.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mn.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aq.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mt.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rt.huanxung.cn

[E14] URL 编码与 Base64
来源：http://cl.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ix.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wd.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cs.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://an.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zr.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xi.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://if.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://py.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://tf.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wq.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ch.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wc.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://df.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zn.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nz.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://in.hahajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ff.shtwfgs.cn

[E16] 数字千分位
来源：http://tl.szsharing.cn

Py:   f"{1234567:,}"
来源：http://fv.colortex.cn

PHP:  number_format(1234567);
来源：http://gv.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jv.panjiajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rb.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hj.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ez.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fl.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://mk.jctech888.com.cn

[E17] 首字母大写
来源：http://tq.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://df.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://km.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hv.nicolike.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dt.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wg.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://di.hahajie.cn

Ruby: s.capitalize
来源：http://tb.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://en.lnxyls.cn

[E18] 模板占位符替换
来源：http://vp.panjiajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bj.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gl.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wp.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ty.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ub.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fx.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vb.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mu.szxytkj.cn

[E19] 多行文本按行拆分
来源：http://zr.yuexingan06.cn

Py:   s.splitlines()
来源：http://ll.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lh.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://ib.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://dp.muxihuayi.cn

Java: s.lines().toList()
来源：http://io.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://xy.huanxung.cn

Ruby: s.lines
来源：http://lr.hnjuh.cn

C#:   s.Split('\n')
来源：http://nc.jianghongdianzi.cn

[E20] 判断字符串是否为空
来源：http://ir.panjiajie.cn

Py:   if not s:
来源：http://wr.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cr.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kb.panjiajie.cn

TS:   if (s === "") {}
来源：http://of.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://dj.shtwfgs.cn

Go:   if s == "" {}
来源：http://ns.chemitech.net.cn

Ruby: if s.empty?
来源：http://tm.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vg.gzmigu.cn

[E21] 超长截断加省略号
来源：http://ry.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dx.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ae.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aq.hnjuh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ue.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pv.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://fq.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cp.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qd.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://as.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vp.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hp.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nl.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lr.newstarts.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ga.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rr.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://da.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xf.huixinmuqiang.cn

================================================================================
来源：http://yo.bookmarksfly.cn

F. 文件与目录
来源：http://zk.lnxyls.cn

================================================================================
来源：http://rr.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://ol.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iu.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://dl.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nv.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zy.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pj.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://my.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://ks.panjiajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://kw.muxihuayi.cn

[F02] 逐行读取文件
来源：http://wf.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://md.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lp.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://he.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yl.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uo.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://df.hnjuh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qa.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://db.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://ga.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ps.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://md.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wg.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ri.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ga.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iw.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://pn.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://re.nicolike.cn

[F04] 追加写入文件
来源：http://cu.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xu.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xk.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cm.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://do.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bi.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sr.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dr.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qw.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://wc.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ol.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://ks.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://en.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://tr.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sj.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vu.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://ls.521024.cn

C#:   File.Exists("a.txt")
来源：http://tw.asd995.cn

[F06] 删除文件
来源：http://qf.9csxet.cn

Py:   os.remove("a.txt")
来源：http://ud.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://py.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tz.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gj.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://iq.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://vo.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://xl.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://fk.szsharing.cn

[F07] 创建目录（含多级）
来源：http://nq.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ws.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dr.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oj.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yn.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qi.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tp.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kp.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tj.lnxyls.cn

[F08] 遍历目录
来源：http://fz.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wr.bjjhwx.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://co.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://zr.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://mj.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hq.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://az.newstarts.cn

Ruby: Dir.children("dir")
来源：http://yk.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://mc.jctech888.com.cn

[F09] 获取文件大小
来源：http://wm.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://lz.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://lf.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://lz.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://df.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mo.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vl.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://ph.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://oz.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://eb.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zd.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ug.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xa.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://yn.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dl.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qr.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tp.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ih.9csxet.cn

[F11] 复制与移动文件
来源：http://md.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kd.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xu.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ir.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pr.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tj.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pb.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ok.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://om.yuexingan06.cn

[F12] CSV 读写
来源：http://ol.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uc.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pf.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sw.lnxyls.cn

TS:   // 同上
来源：http://qm.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://al.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lh.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vn.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ew.bookmarksfly.cn

================================================================================
来源：http://xc.chemitech.net.cn

G. 面向对象
来源：http://dn.shtwfgs.cn

================================================================================
来源：http://cy.wgjwhj.cn

[G01] 定义类
来源：http://vw.wgjwhj.cn

Py:   class User: pass
来源：http://bz.bjjhwx.cn

PHP:  class User {}
来源：http://jf.nicolike.cn

JS:   class User {}
来源：http://ig.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://mw.chemitech.net.cn

Java: class User {}
来源：http://dm.hnjuh.cn

Go:   type User struct { Name string }
来源：http://tj.nicolike.cn

Ruby: class User; end
来源：http://pb.shtwfgs.cn

C#:   class User {}
来源：http://bv.chemitech.net.cn

[G02] 构造函数
来源：http://rf.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://vk.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://ir.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://pm.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://eh.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://kp.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://go.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://mo.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://iz.chemitech.net.cn

[G03] 实例属性
来源：http://eb.huanxung.cn

Py:   self.name = "x"
来源：http://ah.9csxet.cn

PHP:  public string $name = "x";
来源：http://df.huixiangedu.cn


<!-- 参考信息 -->