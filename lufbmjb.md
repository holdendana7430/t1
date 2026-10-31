代发 wailian999

Go:   strings.Index(s, "x")
来源：http://nq.newstarts.cn

Ruby: s.index("x")
来源：http://gc.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://pj.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gj.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zr.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bo.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ho.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xn.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xd.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fy.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ow.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ej.hnjuh.cn

[E06] 替换子串
来源：http://gg.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nb.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://ci.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jp.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://zn.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iv.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://td.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lu.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://sg.gzmigu.cn

[E07] 按分隔符拆分
来源：http://jb.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dm.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vy.9csxet.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fb.nicolike.cn

TS:   s.split(",")
来源：http://lq.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qb.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lo.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://la.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kr.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://xx.yuexingan06.cn

Py:   ",".join(items)
来源：http://nm.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://lu.muxihuayi.cn

JS:   items.join(",")
来源：http://zw.newstarts.cn

TS:   items.join(",")
来源：http://fp.lnxyls.cn

Java: String.join(",", items)
来源：http://on.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://fr.9csxet.cn

Ruby: items.join(",")
来源：http://st.lnxyls.cn

C#:   string.Join(",", items)
来源：http://wa.szxytkj.cn

[E09] 去除所有空白字符
来源：http://wb.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wo.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sf.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://zj.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://sm.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://pq.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dd.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://id.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mq.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://qk.huanxung.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ey.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kj.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://jg.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://jr.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://sl.wgjwhj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pf.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hk.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ts.huixinmuqiang.cn

[E11] 反转字符串
来源：http://fl.szxytkj.cn

Py:   s[::-1]
来源：http://vj.bjjhwx.cn

PHP:  strrev($s);
来源：http://pk.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://zi.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://fo.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://iw.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rc.jctech888.com.cn

Ruby: s.reverse
来源：http://ov.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xi.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://ku.hahajie.cn

Py:   s.count("a")
来源：http://mx.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://ah.yuexingan06.cn

JS:   s.split("a").length - 1
来源：http://zm.nicolike.cn

TS:   s.split("a").length - 1
来源：http://zf.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qk.asd995.cn

Go:   strings.Count(s, "a")
来源：http://xr.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://mp.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://ov.huixiangedu.cn

[E13] 逐字符遍历
来源：http://fg.521024.cn

Py:   for ch in s: print(ch)
来源：http://qk.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fr.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qf.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mo.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fs.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qe.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ve.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hd.szsharing.cn

[E14] URL 编码与 Base64
来源：http://zd.panjiajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sw.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pp.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ob.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xg.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://od.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lh.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sr.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ir.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://ha.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rk.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://te.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kz.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zz.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zg.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pc.gzmigu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ub.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ri.huanxung.cn

[E16] 数字千分位
来源：http://ve.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://mq.lnxyls.cn

PHP:  number_format(1234567);
来源：http://av.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ez.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wb.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ov.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gs.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://es.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://ve.hahajie.cn

[E17] 首字母大写
来源：http://yl.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lj.hnjuh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bg.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ss.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pc.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xk.huixiangedu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nf.nicolike.cn

Ruby: s.capitalize
来源：http://xn.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wc.huixiangedu.cn

[E18] 模板占位符替换
来源：http://ky.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vv.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yr.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wt.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cq.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sr.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bj.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yr.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tc.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://qf.haigaiapp.cn

Py:   s.splitlines()
来源：http://ng.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sh.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://vy.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://yb.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://nt.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://wv.9csxet.cn

Ruby: s.lines
来源：http://eu.chemitech.net.cn

C#:   s.Split('\n')
来源：http://ag.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://zb.nicolike.cn

Py:   if not s:
来源：http://yo.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xq.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tk.asd995.cn

TS:   if (s === "") {}
来源：http://xe.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://ay.panjiajie.cn

Go:   if s == "" {}
来源：http://ui.yuexingan06.cn

Ruby: if s.empty?
来源：http://ap.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sg.panjiajie.cn

[E21] 超长截断加省略号
来源：http://xz.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gs.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rq.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tb.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vb.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yl.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://la.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pl.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mh.hnjuh.cn

[E22] 字节长度与字符长度
来源：http://pt.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wg.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sd.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kj.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://el.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ob.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ne.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://ue.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gw.jianghongdianzi.cn

================================================================================
来源：http://wn.shxzukj.cn

F. 文件与目录
来源：http://aj.jianghongdianzi.cn

================================================================================
来源：http://jl.panjiajie.cn

[F01] 读取整个文件
来源：http://hs.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ub.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://hk.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tr.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ml.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gc.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zo.nicolike.cn

Ruby: File.read("a.txt")
来源：http://jd.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://fi.muxihuayi.cn

[F02] 逐行读取文件
来源：http://hq.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ui.bookmarksfly.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ag.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nw.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lv.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dk.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ts.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lu.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://am.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://eo.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dr.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tb.wgjwhj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bn.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ss.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ul.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ds.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://mr.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qe.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://mq.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ke.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ol.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qo.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gj.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nm.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ci.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nd.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cc.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://hc.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qo.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://tx.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://lc.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://yf.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ra.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gz.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://oo.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://ez.gzmigu.cn

[F06] 删除文件
来源：http://jm.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://vw.nicolike.cn

PHP:  unlink("a.txt");
来源：http://zq.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lz.chemitech.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fn.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bb.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://kq.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://mw.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://wp.szsharing.cn

[F07] 创建目录（含多级）
来源：http://gk.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://at.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bg.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xq.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jk.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bq.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://av.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oq.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ba.shtwfgs.cn

[F08] 遍历目录
来源：http://ha.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kp.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ua.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://ke.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://ia.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gf.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gg.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://ot.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://wm.panjiajie.cn

[F09] 获取文件大小
来源：http://ax.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://do.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://zz.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://lc.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://ik.bookmarksfly.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kn.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ex.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://am.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://cj.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://pm.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pv.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tf.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hr.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://rg.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xo.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zk.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nk.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yn.hnjuh.cn

[F11] 复制与移动文件
来源：http://uz.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aj.jianghongdianzi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cy.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jx.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ad.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vl.szsharing.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fz.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cf.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jr.shxzskj.cn

[F12] CSV 读写
来源：http://rp.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ar.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uv.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rt.newstarts.cn

TS:   // 同上
来源：http://fr.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://il.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sq.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ue.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://va.szxytkj.cn

================================================================================
来源：http://az.yuexingan06.cn

G. 面向对象
来源：http://xm.huixiangedu.cn

================================================================================
来源：http://bv.yuexingan06.cn

[G01] 定义类
来源：http://mh.nszjky.cn

Py:   class User: pass
来源：http://fq.yuexingan06.cn

PHP:  class User {}
来源：http://zz.lnxyls.cn

JS:   class User {}
来源：http://xv.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://gg.asd995.cn

Java: class User {}
来源：http://kk.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://ns.szxytkj.cn

Ruby: class User; end
来源：http://hs.shxzukj.cn

C#:   class User {}
来源：http://tl.gzmigu.cn

[G02] 构造函数
来源：http://hu.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://xz.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://ir.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://li.colortex.cn

TS:   constructor(public name: string) {}
来源：http://rp.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://pv.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tk.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://uk.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://uu.bookmarksfly.cn

[G03] 实例属性
来源：http://rc.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://oc.shtwfgs.cn

PHP:  public string $name = "x";
来源：http://gz.jctech888.com.cn


<!-- 参考信息 -->