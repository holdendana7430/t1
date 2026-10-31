代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://zk.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://kv.nicolike.cn

[E04] 查找子串位置
来源：http://vg.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://to.bjjhwx.cn

PHP:  strpos($s, "x");
来源：http://wu.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qa.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://ni.yuexingan06.cn

Java: s.indexOf("x")
来源：http://gg.521024.cn

Go:   strings.Index(s, "x")
来源：http://ye.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://ko.9csxet.cn

C#:   s.IndexOf("x")
来源：http://yr.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vp.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://me.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ir.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tk.shxzskj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ol.yuntaijiaju.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jq.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kw.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pr.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lx.yuntaijiaju.cn

[E06] 替换子串
来源：http://bg.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yp.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://cu.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qh.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://ds.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xd.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sn.asd995.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ns.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://iu.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://lt.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yc.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xs.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ug.huanxung.cn

TS:   s.split(",")
来源：http://vy.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fl.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ed.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://zm.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qc.asd995.cn

[E08] 数组按分隔符合并
来源：http://hy.hnjuh.cn

Py:   ",".join(items)
来源：http://ow.panjiajie.cn

PHP:  implode(",", $items);
来源：http://hd.newstarts.cn

JS:   items.join(",")
来源：http://wp.shxzskj.cn

TS:   items.join(",")
来源：http://ft.gzmigu.cn

Java: String.join(",", items)
来源：http://et.asd995.cn

Go:   strings.Join(items, ",")
来源：http://xi.hahajie.cn

Ruby: items.join(",")
来源：http://kl.panjiajie.cn

C#:   string.Join(",", items)
来源：http://ah.shxzskj.cn

[E09] 去除所有空白字符
来源：http://pi.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://or.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zn.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://sh.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://sk.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://jj.jianghongdianzi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hw.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ye.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rv.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://rt.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gx.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yq.huixinmuqiang.cn

JS:   "7".padStart(3, "0")
来源：http://qi.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://id.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://tx.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mk.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://me.huixinmuqiang.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wh.9csxet.cn

[E11] 反转字符串
来源：http://uu.huanxung.cn

Py:   s[::-1]
来源：http://ku.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://he.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://dy.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://ta.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xb.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://su.shxzukj.cn

Ruby: s.reverse
来源：http://mm.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pn.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://oo.huanxung.cn

Py:   s.count("a")
来源：http://yt.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://va.hahajie.cn

JS:   s.split("a").length - 1
来源：http://zr.newstarts.cn

TS:   s.split("a").length - 1
来源：http://eb.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dz.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://ym.szxytkj.cn

Ruby: s.count("a")
来源：http://ia.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://wl.shxzukj.cn

[E13] 逐字符遍历
来源：http://zw.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://ot.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tm.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hc.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ce.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rj.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mm.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qn.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dc.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://xz.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tt.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bi.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tv.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tx.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rf.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ur.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ie.haigaiapp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hn.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://ks.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ry.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ms.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://su.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vu.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qd.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tu.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hv.jianghongdianzi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oc.9csxet.cn

[E16] 数字千分位
来源：http://ax.huanxung.cn

Py:   f"{1234567:,}"
来源：http://px.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://ya.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fg.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xz.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vx.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://is.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qa.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://nf.hnjuh.cn

[E17] 首字母大写
来源：http://cd.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pz.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pg.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mv.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tw.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ah.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rx.yuntaijiaju.cn

Ruby: s.capitalize
来源：http://lc.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hv.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://wq.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fl.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yp.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fv.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fi.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tq.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ls.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://to.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fn.hahajie.cn

[E19] 多行文本按行拆分
来源：http://ae.jctech888.com.cn

Py:   s.splitlines()
来源：http://uh.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yi.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://hf.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://ba.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://rf.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://nd.lnxyls.cn

Ruby: s.lines
来源：http://lh.lnxyls.cn

C#:   s.Split('\n')
来源：http://oi.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://kg.jctech888.com.cn

Py:   if not s:
来源：http://ee.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zw.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xa.shxzskj.cn

TS:   if (s === "") {}
来源：http://ng.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://vp.szsharing.cn

Go:   if s == "" {}
来源：http://ze.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://ti.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gh.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://zc.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eu.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ye.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ek.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tz.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://id.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://tb.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eq.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pd.521024.cn

[E22] 字节长度与字符长度
来源：http://lk.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wu.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fl.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://im.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nz.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vg.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sl.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://gc.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yv.szxytkj.cn

================================================================================
来源：http://qw.lnxyls.cn

F. 文件与目录
来源：http://gh.newstarts.cn

================================================================================
来源：http://bw.hnjuh.cn

[F01] 读取整个文件
来源：http://hp.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eh.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://yj.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sl.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://se.521024.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pa.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vh.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://ia.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://sy.shxzskj.cn

[F02] 逐行读取文件
来源：http://rm.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ut.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ku.bjjhwx.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fd.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://je.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wi.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://io.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pa.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zp.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://yv.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dj.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zr.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rx.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xz.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ns.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rl.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://uk.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zp.nicolike.cn

[F04] 追加写入文件
来源：http://vs.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ey.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xl.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gn.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dv.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kc.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://er.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ws.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ev.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://cy.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ba.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://zo.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://ax.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://xy.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://on.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://of.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://ev.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://fw.szxytkj.cn

[F06] 删除文件
来源：http://ui.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://li.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://ly.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lb.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cw.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vp.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://jo.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://ez.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://xd.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://ac.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qk.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fl.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uq.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ks.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ut.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gx.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bi.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://du.haigaiapp.cn

[F08] 遍历目录
来源：http://ct.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gt.yuntaijiaju.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yk.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://lh.521024.cn

TS:   fs.readdirSync("dir")
来源：http://ab.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://po.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lv.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://ve.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://ru.chemitech.net.cn

[F09] 获取文件大小
来源：http://wt.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://uz.nszjky.cn

PHP:  filesize("a.txt");
来源：http://zp.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://tf.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://ne.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vi.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mi.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://lm.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://gf.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://ga.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wq.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ce.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zp.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://or.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kb.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uw.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jk.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dd.hnjuh.cn

[F11] 复制与移动文件
来源：http://eg.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hx.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ia.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://np.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jl.yuntaijiaju.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wz.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yb.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ap.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jv.huixiangedu.cn

[F12] CSV 读写
来源：http://wg.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dd.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xz.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fl.shxzukj.cn

TS:   // 同上
来源：http://at.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lc.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jx.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wj.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pr.shxzukj.cn

================================================================================
来源：http://do.asd995.cn

G. 面向对象
来源：http://ye.colortex.cn

================================================================================
来源：http://kk.lnxyls.cn

[G01] 定义类
来源：http://hy.jctech888.com.cn

Py:   class User: pass
来源：http://zb.gzmigu.cn

PHP:  class User {}
来源：http://fn.shtwfgs.cn

JS:   class User {}
来源：http://bi.521024.cn

TS:   class User { name: string = ""; }
来源：http://xm.huanxung.cn

Java: class User {}
来源：http://dk.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://em.panjiajie.cn

Ruby: class User; end
来源：http://rj.shxzukj.cn

C#:   class User {}
来源：http://vq.szxytkj.cn

[G02] 构造函数
来源：http://ng.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://sa.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://md.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://bc.wgjwhj.cn


<!-- 参考信息 -->