代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://on.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ax.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sn.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ut.yuntaijiaju.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tk.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fi.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eb.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ti.bjjhwx.cn

[E06] 替换子串
来源：http://lw.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pq.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://io.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iq.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://ds.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ob.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wi.asd995.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ab.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://am.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://yg.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eq.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iv.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zt.nicolike.cn

TS:   s.split(",")
来源：http://cq.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sf.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qi.521024.cn

Ruby: s.split(",");  s.split
来源：http://yq.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mt.bjjhwx.cn

[E08] 数组按分隔符合并
来源：http://lq.shxzukj.cn

Py:   ",".join(items)
来源：http://vw.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://ci.yuexingan06.cn

JS:   items.join(",")
来源：http://ew.wgjwhj.cn

TS:   items.join(",")
来源：http://zt.szsharing.cn

Java: String.join(",", items)
来源：http://kj.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://oj.gzmigu.cn

Ruby: items.join(",")
来源：http://sf.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://wa.newstarts.cn

[E09] 去除所有空白字符
来源：http://rj.colortex.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ni.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ez.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://hu.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://vz.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://rz.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rs.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gh.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fz.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://sy.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zx.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tm.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://co.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://dm.asd995.cn

Java: String.format("%03d", 7)
来源：http://ce.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cr.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qh.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gz.huixiangedu.cn

[E11] 反转字符串
来源：http://da.hnjuh.cn

Py:   s[::-1]
来源：http://uw.newstarts.cn

PHP:  strrev($s);
来源：http://fc.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://cy.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://ec.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dw.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wm.huixiangedu.cn

Ruby: s.reverse
来源：http://dz.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ih.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://og.shxzskj.cn

Py:   s.count("a")
来源：http://eg.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://yg.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://ce.haigaiapp.cn

TS:   s.split("a").length - 1
来源：http://bp.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xw.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://nw.gzmigu.cn

Ruby: s.count("a")
来源：http://dt.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://xh.hahajie.cn

[E13] 逐字符遍历
来源：http://ay.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://fb.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://co.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tl.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cl.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://it.yuntaijiaju.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kv.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://to.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xw.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://pc.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ww.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rf.asd995.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://re.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://as.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ty.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iw.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jo.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bs.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://sk.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jx.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cm.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zf.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zc.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jq.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pv.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vd.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hc.hnjuh.cn

[E16] 数字千分位
来源：http://nb.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://ow.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://zr.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://de.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pb.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nh.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wx.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mq.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://ez.lnxyls.cn

[E17] 首字母大写
来源：http://io.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://na.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nc.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xk.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://er.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qf.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xf.bjjhwx.cn

Ruby: s.capitalize
来源：http://hr.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jg.panjiajie.cn

[E18] 模板占位符替换
来源：http://ex.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jj.yuexingan06.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uj.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xi.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bt.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qe.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cz.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hp.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://og.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://uu.shtwfgs.cn

Py:   s.splitlines()
来源：http://ss.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zl.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://al.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://xy.muxihuayi.cn

Java: s.lines().toList()
来源：http://ek.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://tb.huixinmuqiang.cn

Ruby: s.lines
来源：http://ex.szxytkj.cn

C#:   s.Split('\n')
来源：http://wc.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://dr.nszjky.cn

Py:   if not s:
来源：http://pg.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zp.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fs.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://cu.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://oj.shtwfgs.cn

Go:   if s == "" {}
来源：http://lb.nicolike.cn

Ruby: if s.empty?
来源：http://my.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bz.newstarts.cn

[E21] 超长截断加省略号
来源：http://su.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ix.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ii.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oc.chemitech.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ep.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lo.szsharing.cn

Go:   // 按 rune 判断长度后截断
来源：http://uu.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://te.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ex.hahajie.cn

[E22] 字节长度与字符长度
来源：http://ir.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://md.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gt.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bk.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ql.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rj.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qv.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://jk.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sm.szsharing.cn

================================================================================
来源：http://is.9csxet.cn

F. 文件与目录
来源：http://bs.colortex.cn

================================================================================
来源：http://so.lnxyls.cn

[F01] 读取整个文件
来源：http://jm.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fn.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://gb.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tf.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wv.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vz.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qc.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://po.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://hn.shxzukj.cn

[F02] 逐行读取文件
来源：http://kf.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cn.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yc.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zc.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xe.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cb.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pc.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ed.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nd.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://ug.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://to.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sw.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rm.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pb.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ms.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mo.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://jl.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dw.shxzskj.cn

[F04] 追加写入文件
来源：http://bj.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lu.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gm.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ra.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kz.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://em.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yj.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ql.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ob.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://ko.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jb.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://oa.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://jy.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://wz.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bk.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ub.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://wa.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://he.asd995.cn

[F06] 删除文件
来源：http://oc.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://nz.hahajie.cn

PHP:  unlink("a.txt");
来源：http://jp.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uu.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qt.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jb.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://kq.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://cr.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://mv.asd995.cn

[F07] 创建目录（含多级）
来源：http://ly.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tr.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xn.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ae.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ra.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xe.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sf.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hv.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uq.szsharing.cn

[F08] 遍历目录
来源：http://rw.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uc.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zf.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://nq.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://fx.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cz.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sl.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://tj.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://cw.haigaiapp.cn

[F09] 获取文件大小
来源：http://ao.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://bl.asd995.cn

PHP:  filesize("a.txt");
来源：http://ez.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://hm.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://ji.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ih.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xx.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://ly.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://rt.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://ww.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mu.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ll.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cr.colortex.cn

TS:   path.extname("a.txt")
来源：http://dv.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yi.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ou.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gx.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ur.shtwfgs.cn

[F11] 复制与移动文件
来源：http://vs.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mf.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zj.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sc.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qd.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mk.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rx.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ip.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hs.wgjwhj.cn

[F12] CSV 读写
来源：http://mc.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bj.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://du.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ey.nszjky.cn

TS:   // 同上
来源：http://dq.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gx.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rp.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://da.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jz.hahajie.cn

================================================================================
来源：http://tz.shxzskj.cn

G. 面向对象
来源：http://tw.nicolike.cn

================================================================================
来源：http://wy.hahajie.cn

[G01] 定义类
来源：http://mc.szsharing.cn

Py:   class User: pass
来源：http://qt.panjiajie.cn

PHP:  class User {}
来源：http://uj.muxihuayi.cn

JS:   class User {}
来源：http://ns.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://vm.jianghongdianzi.cn

Java: class User {}
来源：http://fp.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://wb.521024.cn

Ruby: class User; end
来源：http://wc.shxzukj.cn

C#:   class User {}
来源：http://fg.chemitech.net.cn

[G02] 构造函数
来源：http://oz.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://su.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://hd.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://js.521024.cn

TS:   constructor(public name: string) {}
来源：http://ee.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://er.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aa.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://ch.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://hv.521024.cn

[G03] 实例属性
来源：http://xl.lnxyls.cn

Py:   self.name = "x"
来源：http://mj.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://bg.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://rc.nszjky.cn

TS:   name: string = "x";
来源：http://gs.panjiajie.cn

Java: private String name;
来源：http://fm.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ct.shxzskj.cn


<!-- 参考信息 -->