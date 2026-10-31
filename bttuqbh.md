代发 wailian999

PHP:  strpos($s, "x");
来源：http://tv.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ag.hnjuh.cn

TS:   s.indexOf("x")
来源：http://xd.jianghongdianzi.cn

Java: s.indexOf("x")
来源：http://bh.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://yh.shxzskj.cn

Ruby: s.index("x")
来源：http://hp.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://at.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vp.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ox.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yj.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iz.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gi.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ly.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nf.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rz.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xp.gzmigu.cn

[E06] 替换子串
来源：http://zk.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ec.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://yl.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ta.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://rf.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ri.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tv.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://if.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://oj.jctech888.com.cn

[E07] 按分隔符拆分
来源：http://au.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bx.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://il.9csxet.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fm.huixiangedu.cn

TS:   s.split(",")
来源：http://nl.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://us.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dp.yuntaijiaju.cn

Ruby: s.split(",");  s.split
来源：http://pk.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eu.bjjhwx.cn

[E08] 数组按分隔符合并
来源：http://vu.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://nh.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://vd.gzmigu.cn

JS:   items.join(",")
来源：http://nz.panjiajie.cn

TS:   items.join(",")
来源：http://ng.muxihuayi.cn

Java: String.join(",", items)
来源：http://ab.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://zq.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://bx.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://nq.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://va.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://am.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://iw.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://id.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://jw.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://jw.jianghongdianzi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sk.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pb.wgjwhj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lx.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://jn.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://if.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ad.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://xl.lnxyls.cn

TS:   "7".padStart(3, "0")
来源：http://fo.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://zg.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jk.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hv.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xc.panjiajie.cn

[E11] 反转字符串
来源：http://ic.szxytkj.cn

Py:   s[::-1]
来源：http://tb.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://ch.lnxyls.cn

JS:   [...s].reverse().join("")
来源：http://es.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://va.asd995.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://oi.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bt.gzmigu.cn

Ruby: s.reverse
来源：http://kr.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ga.9csxet.cn

[E12] 统计某字符出现次数
来源：http://hf.nszjky.cn

Py:   s.count("a")
来源：http://uy.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://nr.yuexingan06.cn

JS:   s.split("a").length - 1
来源：http://ey.nszjky.cn

TS:   s.split("a").length - 1
来源：http://aw.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sm.521024.cn

Go:   strings.Count(s, "a")
来源：http://on.nicolike.cn

Ruby: s.count("a")
来源：http://jv.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://yn.panjiajie.cn

[E13] 逐字符遍历
来源：http://nl.521024.cn

Py:   for ch in s: print(ch)
来源：http://sn.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qr.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cx.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xa.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jr.colortex.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tf.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vy.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://td.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://qq.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pi.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wp.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oj.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pf.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nx.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rt.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pj.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eg.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://il.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hy.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xw.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ni.hnjuh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wx.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://le.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://os.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vr.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xb.chemitech.net.cn

[E16] 数字千分位
来源：http://wr.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://no.shxzskj.cn

PHP:  number_format(1234567);
来源：http://we.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://og.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bg.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yt.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ig.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tc.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://jk.bjjhwx.cn

[E17] 首字母大写
来源：http://fp.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pk.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ci.521024.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ip.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qs.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mg.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jh.bjjhwx.cn

Ruby: s.capitalize
来源：http://jk.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cb.nicolike.cn

[E18] 模板占位符替换
来源：http://qc.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xi.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nv.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zw.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://du.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rb.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pv.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://co.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ah.huanxung.cn

[E19] 多行文本按行拆分
来源：http://my.shxzskj.cn

Py:   s.splitlines()
来源：http://xe.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ry.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://rd.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://ut.hahajie.cn

Java: s.lines().toList()
来源：http://kg.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://fn.panjiajie.cn

Ruby: s.lines
来源：http://is.muxihuayi.cn

C#:   s.Split('\n')
来源：http://gm.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://la.jctech888.com.cn

Py:   if not s:
来源：http://bo.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xq.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cy.yuexingan06.cn

TS:   if (s === "") {}
来源：http://sb.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://mr.huixiangedu.cn

Go:   if s == "" {}
来源：http://tb.521024.cn

Ruby: if s.empty?
来源：http://vl.nicolike.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yq.panjiajie.cn

[E21] 超长截断加省略号
来源：http://ni.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tv.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gb.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jk.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mn.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zh.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://fx.jctech888.com.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ss.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hs.asd995.cn

[E22] 字节长度与字符长度
来源：http://zk.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dv.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ac.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ht.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ol.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hm.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zr.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://it.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tj.newstarts.cn

================================================================================
来源：http://mv.huixiangedu.cn

F. 文件与目录
来源：http://ok.nicolike.cn

================================================================================
来源：http://gh.wgjwhj.cn

[F01] 读取整个文件
来源：http://td.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oq.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://xf.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wh.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vc.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fb.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xm.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://xw.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://ii.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://nt.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cr.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dp.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mk.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ks.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mi.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qj.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ea.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mz.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://ae.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ob.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bb.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kk.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cb.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jq.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lq.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://aa.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://be.jctech888.com.cn

[F04] 追加写入文件
来源：http://jh.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wd.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ak.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lq.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rg.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gb.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pn.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://al.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://et.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://gc.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bd.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://ot.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://li.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://rz.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://og.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dh.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://ej.asd995.cn

C#:   File.Exists("a.txt")
来源：http://re.muxihuayi.cn

[F06] 删除文件
来源：http://yc.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://kx.hahajie.cn

PHP:  unlink("a.txt");
来源：http://vb.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tw.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oz.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xp.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://cz.colortex.cn

Ruby: File.delete("a.txt")
来源：http://zj.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://fz.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://ik.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kw.nicolike.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aa.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bb.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dg.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yn.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ss.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cu.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ax.szsharing.cn

[F08] 遍历目录
来源：http://si.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nk.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oq.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://mo.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://dm.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dy.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wy.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://wg.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://ih.nszjky.cn

[F09] 获取文件大小
来源：http://to.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://bf.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://vr.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://cz.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://ys.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hz.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ni.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://yl.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://dz.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://rv.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ia.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xv.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bv.newstarts.cn

TS:   path.extname("a.txt")
来源：http://pr.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bt.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xd.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uf.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://df.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://tt.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kt.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ui.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dx.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://un.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ef.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hd.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dg.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pq.asd995.cn

[F12] CSV 读写
来源：http://ik.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wv.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://op.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tc.asd995.cn

TS:   // 同上
来源：http://rt.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nx.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://za.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gg.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mq.nicolike.cn

================================================================================
来源：http://dn.shtwfgs.cn

G. 面向对象
来源：http://oz.szxytkj.cn

================================================================================
来源：http://no.huixinmuqiang.cn

[G01] 定义类
来源：http://vp.szsharing.cn

Py:   class User: pass
来源：http://hb.9csxet.cn

PHP:  class User {}
来源：http://mm.colortex.cn

JS:   class User {}
来源：http://xk.colortex.cn

TS:   class User { name: string = ""; }
来源：http://wo.gzmigu.cn

Java: class User {}
来源：http://xl.9csxet.cn

Go:   type User struct { Name string }
来源：http://ia.yuntaijiaju.cn

Ruby: class User; end
来源：http://hu.shxzskj.cn

C#:   class User {}
来源：http://sy.haigaiapp.cn

[G02] 构造函数
来源：http://xs.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://bf.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://us.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://fh.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://hp.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://qs.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wp.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://kv.shtwfgs.cn


<!-- 参考信息 -->