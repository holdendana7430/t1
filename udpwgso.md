代发 wailian999

PHP:  strpos($s, "x");
来源：http://uj.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sf.panjiajie.cn

TS:   s.indexOf("x")
来源：http://oy.panjiajie.cn

Java: s.indexOf("x")
来源：http://nt.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://pj.bookmarksfly.cn

Ruby: s.index("x")
来源：http://sd.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://ru.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qd.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://we.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ku.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ly.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://la.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xo.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cb.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fp.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tj.jianghongdianzi.cn

[E06] 替换子串
来源：http://pu.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kb.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://yt.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kz.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://nf.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gf.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jt.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ur.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://lf.hahajie.cn

[E07] 按分隔符拆分
来源：http://qi.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pz.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://do.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sw.jianghongdianzi.cn

TS:   s.split(",")
来源：http://pt.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xl.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iw.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://iz.yuexingan06.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jj.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://mb.9csxet.cn

Py:   ",".join(items)
来源：http://ge.colortex.cn

PHP:  implode(",", $items);
来源：http://ae.newstarts.cn

JS:   items.join(",")
来源：http://ba.panjiajie.cn

TS:   items.join(",")
来源：http://vo.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://cc.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://xp.jctech888.com.cn

Ruby: items.join(",")
来源：http://pr.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://oy.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://rv.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dv.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qm.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://bd.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://yw.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://fl.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uz.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zd.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cv.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://fh.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mm.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ii.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://lb.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://ty.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://lx.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bf.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ea.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fn.lnxyls.cn

[E11] 反转字符串
来源：http://jq.9csxet.cn

Py:   s[::-1]
来源：http://wg.huixiangedu.cn

PHP:  strrev($s);
来源：http://ni.colortex.cn

JS:   [...s].reverse().join("")
来源：http://za.jctech888.com.cn

TS:   [...s].reverse().join("")
来源：http://eh.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xi.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kp.muxihuayi.cn

Ruby: s.reverse
来源：http://vp.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sm.szsharing.cn

[E12] 统计某字符出现次数
来源：http://bj.huanxung.cn

Py:   s.count("a")
来源：http://ra.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://pc.szsharing.cn

JS:   s.split("a").length - 1
来源：http://gd.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://fe.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ka.asd995.cn

Go:   strings.Count(s, "a")
来源：http://sg.chemitech.net.cn

Ruby: s.count("a")
来源：http://jm.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://ay.muxihuayi.cn

[E13] 逐字符遍历
来源：http://ok.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://bt.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lb.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sy.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zj.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ls.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://as.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://td.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lh.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://hw.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mu.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iq.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ic.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ig.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gv.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ph.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vr.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ce.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://vw.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kp.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wn.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://az.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kg.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wl.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qz.hahajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ip.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rs.521024.cn

[E16] 数字千分位
来源：http://ex.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://jm.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://yf.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fo.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hi.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bn.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pt.colortex.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ra.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://zt.hnjuh.cn

[E17] 首字母大写
来源：http://qs.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ge.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yl.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qv.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fe.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uk.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://et.haigaiapp.cn

Ruby: s.capitalize
来源：http://ug.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bg.muxihuayi.cn

[E18] 模板占位符替换
来源：http://wj.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lp.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kb.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nd.9csxet.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mk.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ni.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kx.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yo.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nj.szsharing.cn

[E19] 多行文本按行拆分
来源：http://hj.shxzukj.cn

Py:   s.splitlines()
来源：http://uo.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cz.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://sj.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://ab.huanxung.cn

Java: s.lines().toList()
来源：http://ot.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://zq.hahajie.cn

Ruby: s.lines
来源：http://sl.shxzskj.cn

C#:   s.Split('\n')
来源：http://ta.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://cs.asd995.cn

Py:   if not s:
来源：http://ad.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vh.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ce.shxzukj.cn

TS:   if (s === "") {}
来源：http://vg.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://br.9csxet.cn

Go:   if s == "" {}
来源：http://lu.newstarts.cn

Ruby: if s.empty?
来源：http://jw.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wx.newstarts.cn

[E21] 超长截断加省略号
来源：http://ed.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://je.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ww.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ij.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ds.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://it.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://nq.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ca.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oj.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://mx.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pt.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eq.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mt.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ev.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://up.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xz.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://iw.gzmigu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ek.yuntaijiaju.cn

================================================================================
来源：http://ac.shxzukj.cn

F. 文件与目录
来源：http://bo.huixiangedu.cn

================================================================================
来源：http://ur.huixiangedu.cn

[F01] 读取整个文件
来源：http://rw.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pg.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://dz.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bh.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yh.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nd.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://im.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://tx.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://pt.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://ps.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oy.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ye.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sm.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pp.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mm.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oy.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://je.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mw.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://he.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pe.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lp.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vh.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zp.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vq.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bc.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://zj.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://es.huanxung.cn

[F04] 追加写入文件
来源：http://qm.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ff.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vv.chemitech.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vw.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rm.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mx.shtwfgs.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ls.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zq.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://om.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://oc.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ao.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://eg.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://pe.huanxung.cn

TS:   fs.existsSync("a.txt")
来源：http://jb.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://na.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pe.jctech888.com.cn

Ruby: File.exist?("a.txt")
来源：http://lt.521024.cn

C#:   File.Exists("a.txt")
来源：http://gb.jianghongdianzi.cn

[F06] 删除文件
来源：http://yl.wgjwhj.cn

Py:   os.remove("a.txt")
来源：http://gm.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://fk.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cv.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lx.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vx.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://jb.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://lj.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://mw.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://fw.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ht.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eb.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jg.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ws.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vz.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fd.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fs.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zt.wgjwhj.cn

[F08] 遍历目录
来源：http://mg.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uo.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fr.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://uh.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://cm.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ct.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qk.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://ue.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://of.huixiangedu.cn

[F09] 获取文件大小
来源：http://cq.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://yx.hahajie.cn

PHP:  filesize("a.txt");
来源：http://mt.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://oc.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://kr.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hw.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://os.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://iw.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://iu.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://ly.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sy.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ci.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://aa.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gc.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mr.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lh.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zz.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://at.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ag.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mm.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://or.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lx.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fu.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pl.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qy.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mj.shtwfgs.cn

[F12] CSV 读写
来源：http://zd.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sr.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hq.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tv.colortex.cn

TS:   // 同上
来源：http://kd.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vq.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ym.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ta.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dz.colortex.cn

================================================================================
来源：http://bw.lnxyls.cn

G. 面向对象
来源：http://ja.gzmigu.cn

================================================================================
来源：http://sf.haigaiapp.cn

[G01] 定义类
来源：http://qx.hahajie.cn

Py:   class User: pass
来源：http://lr.jctech888.com.cn

PHP:  class User {}
来源：http://uf.bjjhwx.cn

JS:   class User {}
来源：http://bo.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://ft.muxihuayi.cn

Java: class User {}
来源：http://sc.szsharing.cn

Go:   type User struct { Name string }
来源：http://ab.hnjuh.cn

Ruby: class User; end
来源：http://jl.gzmigu.cn

C#:   class User {}
来源：http://tn.hahajie.cn

[G02] 构造函数
来源：http://ji.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://ty.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://ka.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://np.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://bc.hnjuh.cn

Java: User(String name) { this.name = name; }
来源：http://dh.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ip.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://yf.huixiangedu.cn


<!-- 参考信息 -->