代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nb.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mb.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://js.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://af.wgjwhj.cn

[E06] 替换子串
来源：http://fr.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lg.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://rh.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hk.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://qa.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qu.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fy.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lb.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://xk.huanxung.cn

[E07] 按分隔符拆分
来源：http://pq.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gf.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://un.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cq.huixinmuqiang.cn

TS:   s.split(",")
来源：http://hg.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qd.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gi.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://dz.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://av.9csxet.cn

[E08] 数组按分隔符合并
来源：http://ak.shxzskj.cn

Py:   ",".join(items)
来源：http://wh.panjiajie.cn

PHP:  implode(",", $items);
来源：http://ft.asd995.cn

JS:   items.join(",")
来源：http://mw.szsharing.cn

TS:   items.join(",")
来源：http://ln.asd995.cn

Java: String.join(",", items)
来源：http://zy.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://ek.shtwfgs.cn

Ruby: items.join(",")
来源：http://da.szsharing.cn

C#:   string.Join(",", items)
来源：http://hn.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://aa.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://df.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ds.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://ze.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://us.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://um.jianghongdianzi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qi.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hl.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://it.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://zd.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zz.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qw.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://dn.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://yx.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://xe.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tp.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cw.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mo.jianghongdianzi.cn

[E11] 反转字符串
来源：http://ky.shxzskj.cn

Py:   s[::-1]
来源：http://rd.panjiajie.cn

PHP:  strrev($s);
来源：http://fq.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://eo.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://yi.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wy.yuexingan06.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dh.gzmigu.cn

Ruby: s.reverse
来源：http://xc.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fb.panjiajie.cn

[E12] 统计某字符出现次数
来源：http://wt.bookmarksfly.cn

Py:   s.count("a")
来源：http://bj.521024.cn

PHP:  substr_count($s, "a");
来源：http://ln.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://ga.haigaiapp.cn

TS:   s.split("a").length - 1
来源：http://ib.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://il.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://pz.haigaiapp.cn

Ruby: s.count("a")
来源：http://ih.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://bb.huanxung.cn

[E13] 逐字符遍历
来源：http://yc.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://ra.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hj.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xi.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rs.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vk.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yi.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://df.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sr.colortex.cn

[E14] URL 编码与 Base64
来源：http://ht.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nx.gzmigu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zd.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sw.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tv.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rg.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jc.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xz.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sy.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://vv.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ue.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zn.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bv.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ou.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vt.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bz.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ph.9csxet.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zg.yuexingan06.cn

[E16] 数字千分位
来源：http://jf.hahajie.cn

Py:   f"{1234567:,}"
来源：http://tf.hahajie.cn

PHP:  number_format(1234567);
来源：http://ph.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://te.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ad.huanxung.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iz.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yj.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jn.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://rb.haigaiapp.cn

[E17] 首字母大写
来源：http://ui.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uc.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vf.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nd.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ob.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rm.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dp.wgjwhj.cn

Ruby: s.capitalize
来源：http://fa.521024.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yy.lnxyls.cn

[E18] 模板占位符替换
来源：http://cl.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ss.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ln.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sa.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hu.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xs.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zd.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ry.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://th.newstarts.cn

[E19] 多行文本按行拆分
来源：http://wl.nszjky.cn

Py:   s.splitlines()
来源：http://tl.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xn.521024.cn

JS:   s.split(/\r?\n/)
来源：http://fs.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://qj.muxihuayi.cn

Java: s.lines().toList()
来源：http://dw.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://ly.bookmarksfly.cn

Ruby: s.lines
来源：http://jf.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://gg.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://xb.szsharing.cn

Py:   if not s:
来源：http://wx.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qb.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vb.huanxung.cn

TS:   if (s === "") {}
来源：http://bk.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://lg.muxihuayi.cn

Go:   if s == "" {}
来源：http://wr.jctech888.com.cn

Ruby: if s.empty?
来源：http://ll.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hx.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://gz.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ei.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ik.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vx.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cj.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hs.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://fs.jianghongdianzi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lq.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://on.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://aa.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lp.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://np.huixiangedu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ja.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pp.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kn.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sf.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://es.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iz.huixinmuqiang.cn

================================================================================
来源：http://eq.hahajie.cn

F. 文件与目录
来源：http://ae.huixiangedu.cn

================================================================================
来源：http://lr.lnxyls.cn

[F01] 读取整个文件
来源：http://sr.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hd.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://kp.chemitech.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hr.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wl.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ac.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sz.hahajie.cn

Ruby: File.read("a.txt")
来源：http://ne.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://hv.521024.cn

[F02] 逐行读取文件
来源：http://su.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cc.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dv.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vb.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rc.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oo.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gt.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dt.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qs.521024.cn

[F03] 写入文件（覆盖）
来源：http://iw.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jf.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mc.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nu.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ye.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xc.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ni.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://pq.lnxyls.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hp.panjiajie.cn

[F04] 追加写入文件
来源：http://bb.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wo.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bx.huixinmuqiang.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aw.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tt.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ej.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ts.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hd.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lc.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://ko.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ab.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://ju.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://on.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://vk.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wt.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nd.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://mn.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://jz.haigaiapp.cn

[F06] 删除文件
来源：http://fy.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://hc.9csxet.cn

PHP:  unlink("a.txt");
来源：http://gk.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nm.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mx.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://il.asd995.cn

Go:   os.Remove("a.txt")
来源：http://hy.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://xh.asd995.cn

C#:   File.Delete("a.txt");
来源：http://yl.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://qw.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qa.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fs.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://im.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uo.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rm.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wa.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://az.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kk.nicolike.cn

[F08] 遍历目录
来源：http://xn.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xw.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ml.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://fj.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://oy.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fc.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sb.newstarts.cn

Ruby: Dir.children("dir")
来源：http://wt.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://wv.hahajie.cn

[F09] 获取文件大小
来源：http://oo.hahajie.cn

Py:   os.path.getsize("a.txt")
来源：http://ex.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://cz.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://nt.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://wx.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nn.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dj.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://pu.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://eu.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://dn.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fj.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hq.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pj.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://rt.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mh.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ov.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cp.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nd.huanxung.cn

[F11] 复制与移动文件
来源：http://xz.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://js.bjjhwx.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ax.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wh.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ni.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lq.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vb.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zd.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tp.newstarts.cn

[F12] CSV 读写
来源：http://ag.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mn.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ux.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gr.yuexingan06.cn

TS:   // 同上
来源：http://ma.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fq.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ca.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qa.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xz.lnxyls.cn

================================================================================
来源：http://qo.huixiangedu.cn

G. 面向对象
来源：http://ni.shxzukj.cn

================================================================================
来源：http://gp.hnjuh.cn

[G01] 定义类
来源：http://so.huixiangedu.cn

Py:   class User: pass
来源：http://fm.panjiajie.cn

PHP:  class User {}
来源：http://jp.huanxung.cn

JS:   class User {}
来源：http://zc.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://cb.yuntaijiaju.cn

Java: class User {}
来源：http://sx.szxytkj.cn

Go:   type User struct { Name string }
来源：http://ym.nicolike.cn

Ruby: class User; end
来源：http://hq.nszjky.cn

C#:   class User {}
来源：http://eg.bookmarksfly.cn

[G02] 构造函数
来源：http://kf.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://jv.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://md.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://rf.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://xh.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://cp.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tw.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://vu.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://ji.shtwfgs.cn

[G03] 实例属性
来源：http://pc.shxzukj.cn

Py:   self.name = "x"
来源：http://br.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://rv.asd995.cn

JS:   this.name = "x";
来源：http://ls.panjiajie.cn

TS:   name: string = "x";
来源：http://cq.haigaiapp.cn

Java: private String name;
来源：http://kd.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wg.panjiajie.cn

Ruby: @name = "x"
来源：http://lu.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://ps.muxihuayi.cn

[G04] 定义方法
来源：http://ki.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://zo.yuexingan06.cn


<!-- 参考信息 -->