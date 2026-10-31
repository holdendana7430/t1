代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dh.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fx.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ll.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mu.newstarts.cn

[E06] 替换子串
来源：http://ke.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pa.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://px.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sq.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://hg.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lk.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bz.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wa.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://rk.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://ir.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vp.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hk.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sn.nszjky.cn

TS:   s.split(",")
来源：http://zi.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ie.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hr.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://ju.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://io.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://hx.colortex.cn

Py:   ",".join(items)
来源：http://dv.szsharing.cn

PHP:  implode(",", $items);
来源：http://kp.jctech888.com.cn

JS:   items.join(",")
来源：http://ha.huixiangedu.cn

TS:   items.join(",")
来源：http://jm.bookmarksfly.cn

Java: String.join(",", items)
来源：http://jn.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://jr.asd995.cn

Ruby: items.join(",")
来源：http://bm.shxzukj.cn

C#:   string.Join(",", items)
来源：http://ch.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://ui.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rl.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://si.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://iz.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://qz.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://lf.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lk.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tn.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kh.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://gl.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://th.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wf.huixinmuqiang.cn

JS:   "7".padStart(3, "0")
来源：http://hi.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://ww.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://mk.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pz.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qh.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nx.bookmarksfly.cn

[E11] 反转字符串
来源：http://is.9csxet.cn

Py:   s[::-1]
来源：http://jv.szsharing.cn

PHP:  strrev($s);
来源：http://wm.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://yv.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://nd.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tw.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zo.huixiangedu.cn

Ruby: s.reverse
来源：http://mh.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xr.9csxet.cn

[E12] 统计某字符出现次数
来源：http://lm.muxihuayi.cn

Py:   s.count("a")
来源：http://pz.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://ns.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://di.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://sj.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://su.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://id.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://gl.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://nh.huixiangedu.cn

[E13] 逐字符遍历
来源：http://sx.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://fv.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ho.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tb.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://he.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fk.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xo.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jb.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fl.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://nm.hahajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ug.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mg.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qp.nicolike.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fx.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ot.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mh.shxzskj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://op.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tp.521024.cn

[E15] HTML 转义 / 反转义
来源：http://wa.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xp.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oj.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tt.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ew.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zy.wgjwhj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ud.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://au.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ta.hahajie.cn

[E16] 数字千分位
来源：http://mh.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://dc.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://ch.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qu.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://px.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uz.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yy.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oh.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://wl.shtwfgs.cn

[E17] 首字母大写
来源：http://hg.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qh.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rc.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uz.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dj.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bb.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ft.shxzukj.cn

Ruby: s.capitalize
来源：http://rm.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xu.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://sh.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sq.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yt.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ug.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qk.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xk.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uj.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wa.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zf.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://iq.szxytkj.cn

Py:   s.splitlines()
来源：http://ye.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gr.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://hx.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://do.hahajie.cn

Java: s.lines().toList()
来源：http://fd.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://fn.asd995.cn

Ruby: s.lines
来源：http://si.panjiajie.cn

C#:   s.Split('\n')
来源：http://cv.hahajie.cn

[E20] 判断字符串是否为空
来源：http://fi.nszjky.cn

Py:   if not s:
来源：http://zd.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gr.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jk.521024.cn

TS:   if (s === "") {}
来源：http://ab.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://oj.szsharing.cn

Go:   if s == "" {}
来源：http://tq.lnxyls.cn

Ruby: if s.empty?
来源：http://so.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://px.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://se.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bu.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ul.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pb.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ux.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qu.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://av.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yu.newstarts.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rl.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://so.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ld.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fh.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wr.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://od.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qy.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pp.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://ch.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uo.shxzukj.cn

================================================================================
来源：http://we.chemitech.net.cn

F. 文件与目录
来源：http://mm.nszjky.cn

================================================================================
来源：http://cx.hahajie.cn

[F01] 读取整个文件
来源：http://qb.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ku.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://he.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zn.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zv.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jp.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ak.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://ki.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://kc.yuexingan06.cn

[F02] 逐行读取文件
来源：http://kr.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yo.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pv.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pa.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qo.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ny.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ee.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iv.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://no.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://gp.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lu.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xh.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hc.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://id.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://up.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tj.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://ny.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://js.gzmigu.cn

[F04] 追加写入文件
来源：http://li.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sq.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ci.colortex.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kp.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nn.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://co.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ef.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pu.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ec.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://rb.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ob.521024.cn

PHP:  file_exists("a.txt");
来源：http://vs.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://pa.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://wb.lnxyls.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://me.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rg.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://mv.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://eh.yuntaijiaju.cn

[F06] 删除文件
来源：http://pq.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://kh.hahajie.cn

PHP:  unlink("a.txt");
来源：http://ru.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kq.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nv.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sy.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://zv.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://uy.asd995.cn

C#:   File.Delete("a.txt");
来源：http://fv.huanxung.cn

[F07] 创建目录（含多级）
来源：http://uq.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ox.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mr.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ck.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wy.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hk.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jn.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://og.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eb.haigaiapp.cn

[F08] 遍历目录
来源：http://tk.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ey.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ql.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://dw.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://in.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yc.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dv.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://at.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://es.szxytkj.cn

[F09] 获取文件大小
来源：http://hc.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://jq.521024.cn

PHP:  filesize("a.txt");
来源：http://li.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://vr.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://qx.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rs.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://an.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://sh.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://dq.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://gh.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ku.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://db.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jw.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://mt.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qq.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xh.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ss.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oq.colortex.cn

[F11] 复制与移动文件
来源：http://ys.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://co.jianghongdianzi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lg.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lm.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mh.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wy.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://el.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sk.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jx.nicolike.cn

[F12] CSV 读写
来源：http://pd.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://va.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://po.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yj.lnxyls.cn

TS:   // 同上
来源：http://cu.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jd.huanxung.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xk.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zy.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tx.panjiajie.cn

================================================================================
来源：http://id.bjjhwx.cn

G. 面向对象
来源：http://ca.shxzukj.cn

================================================================================
来源：http://bl.bjjhwx.cn

[G01] 定义类
来源：http://bo.haigaiapp.cn

Py:   class User: pass
来源：http://bj.yuntaijiaju.cn

PHP:  class User {}
来源：http://po.szxytkj.cn

JS:   class User {}
来源：http://so.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://fy.gzmigu.cn

Java: class User {}
来源：http://fa.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://zn.shxzskj.cn

Ruby: class User; end
来源：http://wg.bjjhwx.cn

C#:   class User {}
来源：http://mp.jianghongdianzi.cn

[G02] 构造函数
来源：http://ul.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://mz.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://so.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://zn.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://st.shtwfgs.cn

Java: User(String name) { this.name = name; }
来源：http://jc.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zr.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://cc.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://hz.nszjky.cn

[G03] 实例属性
来源：http://gb.bookmarksfly.cn

Py:   self.name = "x"
来源：http://nu.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://hb.yuexingan06.cn

JS:   this.name = "x";
来源：http://ns.hahajie.cn

TS:   name: string = "x";
来源：http://rd.hahajie.cn

Java: private String name;
来源：http://vx.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rd.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://mh.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://vh.nicolike.cn

[G04] 定义方法
来源：http://ta.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://hv.yuntaijiaju.cn


<!-- 参考信息 -->