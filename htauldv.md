代发 wailian999

PHP:  strpos($s, "x");
来源：http://jf.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ay.521024.cn

TS:   s.indexOf("x")
来源：http://qh.gzmigu.cn

Java: s.indexOf("x")
来源：http://wu.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://ep.szxytkj.cn

Ruby: s.index("x")
来源：http://hy.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://kr.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ow.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nu.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qt.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vq.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qp.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mn.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wh.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ts.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lu.jctech888.com.cn

[E06] 替换子串
来源：http://ia.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hs.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://gq.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lg.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://gx.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pu.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sw.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qn.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://ys.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://ls.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cp.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cz.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cq.haigaiapp.cn

TS:   s.split(",")
来源：http://rt.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cp.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bu.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://cc.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fg.asd995.cn

[E08] 数组按分隔符合并
来源：http://dt.bookmarksfly.cn

Py:   ",".join(items)
来源：http://ak.lnxyls.cn

PHP:  implode(",", $items);
来源：http://wb.panjiajie.cn

JS:   items.join(",")
来源：http://pp.muxihuayi.cn

TS:   items.join(",")
来源：http://bt.521024.cn

Java: String.join(",", items)
来源：http://pp.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://hg.colortex.cn

Ruby: items.join(",")
来源：http://xh.nszjky.cn

C#:   string.Join(",", items)
来源：http://pm.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://tn.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xc.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uh.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://hd.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://mk.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://ex.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sm.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gc.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zv.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://uk.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hn.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fz.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://wj.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://vn.hahajie.cn

Java: String.format("%03d", 7)
来源：http://cu.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jx.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dh.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ik.panjiajie.cn

[E11] 反转字符串
来源：http://ak.hnjuh.cn

Py:   s[::-1]
来源：http://kj.gzmigu.cn

PHP:  strrev($s);
来源：http://vc.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://ky.panjiajie.cn

TS:   [...s].reverse().join("")
来源：http://pc.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mn.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tw.lnxyls.cn

Ruby: s.reverse
来源：http://ff.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qy.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://yw.jianghongdianzi.cn

Py:   s.count("a")
来源：http://jw.huixiangedu.cn

PHP:  substr_count($s, "a");
来源：http://sq.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://pu.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://qa.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://do.colortex.cn

Go:   strings.Count(s, "a")
来源：http://qq.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://jv.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://sb.shxzukj.cn

[E13] 逐字符遍历
来源：http://zi.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://of.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://si.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fo.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mx.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ls.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ql.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nw.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jl.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://kx.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rp.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ri.hnjuh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qr.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://de.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ld.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oa.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ym.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mk.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://ft.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://oq.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://su.jianghongdianzi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aq.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ln.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pq.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sa.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pq.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oj.huanxung.cn

[E16] 数字千分位
来源：http://dh.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://fn.nicolike.cn

PHP:  number_format(1234567);
来源：http://sc.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lc.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gl.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gi.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yh.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tm.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://eu.bookmarksfly.cn

[E17] 首字母大写
来源：http://wu.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lh.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vc.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qe.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fx.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sy.huixiangedu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://if.lnxyls.cn

Ruby: s.capitalize
来源：http://dx.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hj.huanxung.cn

[E18] 模板占位符替换
来源：http://pb.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uu.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bs.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jp.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tb.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gn.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ba.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cm.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uw.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://id.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://vh.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cg.chemitech.net.cn

JS:   s.split(/\r?\n/)
来源：http://sj.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://aw.panjiajie.cn

Java: s.lines().toList()
来源：http://cp.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://zj.huanxung.cn

Ruby: s.lines
来源：http://xx.panjiajie.cn

C#:   s.Split('\n')
来源：http://sp.shxzskj.cn

[E20] 判断字符串是否为空
来源：http://bj.huixinmuqiang.cn

Py:   if not s:
来源：http://xj.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qp.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yy.hnjuh.cn

TS:   if (s === "") {}
来源：http://xi.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://qz.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://bc.panjiajie.cn

Ruby: if s.empty?
来源：http://xc.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xs.521024.cn

[E21] 超长截断加省略号
来源：http://sb.shxzukj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bq.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ji.huixiangedu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ok.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://km.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gg.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://fp.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sx.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ex.nicolike.cn

[E22] 字节长度与字符长度
来源：http://nm.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://au.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iz.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tb.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jn.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ar.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qd.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://jw.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qc.muxihuayi.cn

================================================================================
来源：http://de.muxihuayi.cn

F. 文件与目录
来源：http://ix.shtwfgs.cn

================================================================================
来源：http://oo.huixiangedu.cn

[F01] 读取整个文件
来源：http://nl.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://et.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://rg.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://im.asd995.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cx.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qj.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ll.jctech888.com.cn

Ruby: File.read("a.txt")
来源：http://ey.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://sc.521024.cn

[F02] 逐行读取文件
来源：http://rs.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bz.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dr.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pq.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rm.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ts.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://id.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xi.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nf.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://mv.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jb.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mg.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hx.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wq.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gl.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vm.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://uk.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qr.jctech888.com.cn

[F04] 追加写入文件
来源：http://au.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ih.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vs.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zm.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://re.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dy.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wz.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qf.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pz.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://wn.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pf.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://eg.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://hw.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://qv.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hm.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bd.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://jq.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://ye.shtwfgs.cn

[F06] 删除文件
来源：http://rs.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://pn.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://ke.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jl.chemitech.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://po.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bp.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://zi.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://kw.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://jy.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://bd.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sg.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xg.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yx.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ye.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lj.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ff.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ku.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tr.jctech888.com.cn

[F08] 遍历目录
来源：http://xw.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vw.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aq.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://mv.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://ce.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://si.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pk.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://ci.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://cw.szsharing.cn

[F09] 获取文件大小
来源：http://ck.jianghongdianzi.cn

Py:   os.path.getsize("a.txt")
来源：http://hc.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://yq.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://ef.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://kr.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yk.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yf.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://ve.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://nr.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://zt.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fi.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gm.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://my.nicolike.cn

TS:   path.extname("a.txt")
来源：http://af.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://js.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xq.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gu.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iq.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://dx.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qh.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iu.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ga.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fn.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dq.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gh.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hq.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fc.nszjky.cn

[F12] CSV 读写
来源：http://jk.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hn.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lj.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tq.nicolike.cn

TS:   // 同上
来源：http://lb.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ng.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://va.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eb.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ou.wgjwhj.cn

================================================================================
来源：http://ru.colortex.cn

G. 面向对象
来源：http://vc.chemitech.net.cn

================================================================================
来源：http://dg.nicolike.cn

[G01] 定义类
来源：http://nn.bookmarksfly.cn

Py:   class User: pass
来源：http://sc.9csxet.cn

PHP:  class User {}
来源：http://gi.bookmarksfly.cn

JS:   class User {}
来源：http://uq.szsharing.cn

TS:   class User { name: string = ""; }
来源：http://ih.jctech888.com.cn

Java: class User {}
来源：http://xr.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://xb.colortex.cn

Ruby: class User; end
来源：http://rw.muxihuayi.cn

C#:   class User {}
来源：http://tq.bjjhwx.cn

[G02] 构造函数
来源：http://bi.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://tz.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://ng.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://po.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://tz.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://xo.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pv.9csxet.cn

Ruby: def initialize(name); @name = name; end
来源：http://pr.bookmarksfly.cn


<!-- 参考信息 -->