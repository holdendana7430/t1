代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://bz.gzmigu.cn

C#:   s.Substring(1, 3)
来源：http://sh.haigaiapp.cn

[E04] 查找子串位置
来源：http://bw.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://ye.huanxung.cn

PHP:  strpos($s, "x");
来源：http://hc.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gb.szxytkj.cn

TS:   s.indexOf("x")
来源：http://wj.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://ql.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://nv.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://zw.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://mn.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://li.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xg.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jj.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zc.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ri.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rc.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kh.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ir.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ch.shxzskj.cn

[E06] 替换子串
来源：http://qx.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://og.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://kf.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gm.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://lx.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hi.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gq.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dq.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://es.shxzskj.cn

[E07] 按分隔符拆分
来源：http://yz.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jb.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vs.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cl.jianghongdianzi.cn

TS:   s.split(",")
来源：http://th.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://on.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qd.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://sr.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xu.nszjky.cn

[E08] 数组按分隔符合并
来源：http://zx.wgjwhj.cn

Py:   ",".join(items)
来源：http://ub.colortex.cn

PHP:  implode(",", $items);
来源：http://fi.shxzukj.cn

JS:   items.join(",")
来源：http://wb.9csxet.cn

TS:   items.join(",")
来源：http://rc.521024.cn

Java: String.join(",", items)
来源：http://yw.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://cq.gzmigu.cn

Ruby: items.join(",")
来源：http://eu.521024.cn

C#:   string.Join(",", items)
来源：http://bs.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://sy.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jb.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://og.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://ce.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://dk.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://jm.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ks.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qn.wgjwhj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pg.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://mm.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ic.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://la.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://qy.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://ee.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://on.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ol.colortex.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ky.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sl.chemitech.net.cn

[E11] 反转字符串
来源：http://ut.muxihuayi.cn

Py:   s[::-1]
来源：http://il.huanxung.cn

PHP:  strrev($s);
来源：http://zo.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://zo.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://pl.huixiangedu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sk.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vw.huanxung.cn

Ruby: s.reverse
来源：http://vq.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ku.nszjky.cn

[E12] 统计某字符出现次数
来源：http://lj.9csxet.cn

Py:   s.count("a")
来源：http://ep.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://xu.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://bl.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://gb.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hw.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://xk.lnxyls.cn

Ruby: s.count("a")
来源：http://sh.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://ej.521024.cn

[E13] 逐字符遍历
来源：http://ew.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://ka.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bc.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nw.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://si.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vk.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://js.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sw.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fj.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://qd.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tk.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lw.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zh.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nf.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fj.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xq.hnjuh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hw.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rs.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://jx.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kb.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ck.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jh.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mg.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hf.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://aq.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cr.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://go.hahajie.cn

[E16] 数字千分位
来源：http://wj.colortex.cn

Py:   f"{1234567:,}"
来源：http://ra.lnxyls.cn

PHP:  number_format(1234567);
来源：http://dc.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mi.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jc.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vl.gzmigu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qv.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hi.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://ld.chemitech.net.cn

[E17] 首字母大写
来源：http://ur.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://an.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vn.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bm.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fr.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qb.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ax.nicolike.cn

Ruby: s.capitalize
来源：http://bc.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dt.newstarts.cn

[E18] 模板占位符替换
来源：http://ah.shxzukj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zb.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ps.shxzskj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://na.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ic.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ju.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yd.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ff.lnxyls.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://og.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://io.wgjwhj.cn

Py:   s.splitlines()
来源：http://ge.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cv.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://ql.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://eu.nszjky.cn

Java: s.lines().toList()
来源：http://hp.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://qy.huixiangedu.cn

Ruby: s.lines
来源：http://is.bjjhwx.cn

C#:   s.Split('\n')
来源：http://ja.jianghongdianzi.cn

[E20] 判断字符串是否为空
来源：http://ov.huanxung.cn

Py:   if not s:
来源：http://zg.chemitech.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hv.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nz.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://wl.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://cb.shxzskj.cn

Go:   if s == "" {}
来源：http://xl.newstarts.cn

Ruby: if s.empty?
来源：http://gq.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oe.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://bc.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hc.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vs.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dz.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fj.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cd.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://rd.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kc.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wg.hahajie.cn

[E22] 字节长度与字符长度
来源：http://oi.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ex.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ve.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vx.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ja.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qe.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://om.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://vu.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ul.huixiangedu.cn

================================================================================
来源：http://kw.panjiajie.cn

F. 文件与目录
来源：http://ov.bookmarksfly.cn

================================================================================
来源：http://uf.colortex.cn

[F01] 读取整个文件
来源：http://yd.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://km.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://hm.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hw.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iz.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://br.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pm.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://lo.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://bc.newstarts.cn

[F02] 逐行读取文件
来源：http://cp.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fz.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sx.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ld.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uu.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uq.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qp.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ni.nszjky.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ps.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://ls.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cn.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nq.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lo.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gf.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wb.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qn.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://rt.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vk.hnjuh.cn

[F04] 追加写入文件
来源：http://fg.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oc.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qk.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pt.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ln.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rl.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ac.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ni.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ss.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://qu.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bd.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://tm.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://sm.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://tx.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mv.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iu.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://yb.nicolike.cn

C#:   File.Exists("a.txt")
来源：http://gh.lnxyls.cn

[F06] 删除文件
来源：http://id.521024.cn

Py:   os.remove("a.txt")
来源：http://hm.9csxet.cn

PHP:  unlink("a.txt");
来源：http://vf.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vn.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qx.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dv.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://ai.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://hl.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://fq.huanxung.cn

[F07] 创建目录（含多级）
来源：http://iq.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tq.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tl.huixinmuqiang.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bc.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ei.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://go.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ju.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sy.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vr.hahajie.cn

[F08] 遍历目录
来源：http://zp.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vr.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ms.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://he.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://it.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tr.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vt.huixiangedu.cn

Ruby: Dir.children("dir")
来源：http://sf.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://fe.huixiangedu.cn

[F09] 获取文件大小
来源：http://uc.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://rf.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://qw.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://rc.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://ix.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pu.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ey.nicolike.cn

Ruby: File.size("a.txt")
来源：http://yc.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://oi.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://zy.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ie.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jx.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yk.newstarts.cn

TS:   path.extname("a.txt")
来源：http://gd.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jx.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://md.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nq.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nz.panjiajie.cn

[F11] 复制与移动文件
来源：http://jl.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://od.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://on.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zi.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qb.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aw.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hc.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://os.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xr.9csxet.cn

[F12] CSV 读写
来源：http://dk.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uz.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://be.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://en.huanxung.cn

TS:   // 同上
来源：http://la.colortex.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ej.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://og.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xs.9csxet.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qz.521024.cn

================================================================================
来源：http://of.huixiangedu.cn

G. 面向对象
来源：http://qn.bookmarksfly.cn

================================================================================
来源：http://vc.wgjwhj.cn

[G01] 定义类
来源：http://ow.jianghongdianzi.cn

Py:   class User: pass
来源：http://aq.shtwfgs.cn

PHP:  class User {}
来源：http://bc.colortex.cn

JS:   class User {}
来源：http://hr.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://ed.521024.cn

Java: class User {}
来源：http://yw.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://he.jianghongdianzi.cn

Ruby: class User; end
来源：http://dr.colortex.cn

C#:   class User {}
来源：http://oq.jianghongdianzi.cn

[G02] 构造函数
来源：http://on.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://ns.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://zb.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://ou.shtwfgs.cn


<!-- 参考信息 -->