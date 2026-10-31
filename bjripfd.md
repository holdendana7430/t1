代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hh.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fs.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nq.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zc.jianghongdianzi.cn

[E06] 替换子串
来源：http://rt.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xb.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://sy.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cy.hnjuh.cn

TS:   s.replaceAll("a", "b")
来源：http://dc.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gm.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sc.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cp.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://gz.asd995.cn

[E07] 按分隔符拆分
来源：http://ve.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sq.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hd.yuexingan06.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ea.lnxyls.cn

TS:   s.split(",")
来源：http://xf.szxytkj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sg.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ks.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://jm.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lw.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://de.lnxyls.cn

Py:   ",".join(items)
来源：http://ab.asd995.cn

PHP:  implode(",", $items);
来源：http://ez.yuntaijiaju.cn

JS:   items.join(",")
来源：http://jz.nszjky.cn

TS:   items.join(",")
来源：http://ep.521024.cn

Java: String.join(",", items)
来源：http://ym.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://dd.chemitech.net.cn

Ruby: items.join(",")
来源：http://fx.shxzukj.cn

C#:   string.Join(",", items)
来源：http://zi.521024.cn

[E09] 去除所有空白字符
来源：http://oo.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fo.huixinmuqiang.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qp.hahajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://qq.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://wq.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://ja.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rc.huixinmuqiang.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uu.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fy.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://bk.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mh.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gt.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://mx.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://ci.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://cu.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pd.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ja.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fg.colortex.cn

[E11] 反转字符串
来源：http://uq.yuexingan06.cn

Py:   s[::-1]
来源：http://ft.panjiajie.cn

PHP:  strrev($s);
来源：http://aj.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://hu.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://ev.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dd.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qx.jctech888.com.cn

Ruby: s.reverse
来源：http://dj.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://et.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://oy.jianghongdianzi.cn

Py:   s.count("a")
来源：http://kg.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://yv.shxzukj.cn

JS:   s.split("a").length - 1
来源：http://qi.huanxung.cn

TS:   s.split("a").length - 1
来源：http://bc.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://av.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://dx.hnjuh.cn

Ruby: s.count("a")
来源：http://us.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://zw.shxzukj.cn

[E13] 逐字符遍历
来源：http://ik.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://tz.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qu.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sm.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mw.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wy.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xo.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://on.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yh.huanxung.cn

[E14] URL 编码与 Base64
来源：http://mn.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yl.gzmigu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jz.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ly.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://su.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dn.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jl.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kg.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eq.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://gw.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://my.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bq.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kk.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jj.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lt.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kq.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fu.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bf.chemitech.net.cn

[E16] 数字千分位
来源：http://hq.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://id.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://bb.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bl.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rg.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vx.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jd.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bo.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://jy.panjiajie.cn

[E17] 首字母大写
来源：http://dc.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sy.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gv.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://al.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xc.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mi.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uu.colortex.cn

Ruby: s.capitalize
来源：http://mq.521024.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hm.nicolike.cn

[E18] 模板占位符替换
来源：http://xg.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wd.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vj.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ke.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ao.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://te.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pg.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pq.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lz.nicolike.cn

[E19] 多行文本按行拆分
来源：http://ik.colortex.cn

Py:   s.splitlines()
来源：http://yy.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jw.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://xd.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://yr.yuexingan06.cn

Java: s.lines().toList()
来源：http://rc.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://lv.huixiangedu.cn

Ruby: s.lines
来源：http://cx.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://ml.huanxung.cn

[E20] 判断字符串是否为空
来源：http://mb.huixiangedu.cn

Py:   if not s:
来源：http://pd.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fj.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ke.chemitech.net.cn

TS:   if (s === "") {}
来源：http://mc.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://jp.yuexingan06.cn

Go:   if s == "" {}
来源：http://eo.szxytkj.cn

Ruby: if s.empty?
来源：http://rz.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vs.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://gs.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ny.wgjwhj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eg.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://re.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qc.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wp.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://tt.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kl.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hp.nszjky.cn

[E22] 字节长度与字符长度
来源：http://em.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xc.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ey.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tj.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://no.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kx.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ry.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://jg.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ba.huixiangedu.cn

================================================================================
来源：http://jr.chemitech.net.cn

F. 文件与目录
来源：http://jt.shtwfgs.cn

================================================================================
来源：http://qe.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://mz.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uz.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://uv.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bp.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qo.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nm.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://no.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://lr.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://tr.shxzukj.cn

[F02] 逐行读取文件
来源：http://fk.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rw.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://go.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tu.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ki.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ob.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zc.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://np.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pb.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://wh.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ce.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ua.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fy.hnjuh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tt.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xt.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pa.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://rg.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lz.newstarts.cn

[F04] 追加写入文件
来源：http://ka.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ny.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ga.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mb.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://br.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nj.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gp.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gu.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://et.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://wf.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://im.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://pj.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://bo.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://cs.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://up.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xt.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://up.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://cz.gzmigu.cn

[F06] 删除文件
来源：http://jd.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://bh.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://rr.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yv.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zr.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ak.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://lr.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://uf.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://xn.asd995.cn

[F07] 创建目录（含多级）
来源：http://ax.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xq.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lu.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ue.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://og.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bc.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vm.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mt.huanxung.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rg.newstarts.cn

[F08] 遍历目录
来源：http://wq.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uu.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pa.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://xd.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://ud.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qj.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://df.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://ey.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://ky.wgjwhj.cn

[F09] 获取文件大小
来源：http://zk.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://ry.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://yq.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://ao.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://wt.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pb.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qq.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://wg.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://ph.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://bz.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sf.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zd.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ln.nszjky.cn

TS:   path.extname("a.txt")
来源：http://ka.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ua.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dd.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kv.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dx.wgjwhj.cn

[F11] 复制与移动文件
来源：http://by.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vy.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xn.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://we.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ht.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qm.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gk.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zc.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uc.shxzukj.cn

[F12] CSV 读写
来源：http://wf.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ii.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qy.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kl.lnxyls.cn

TS:   // 同上
来源：http://xz.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://du.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ir.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ih.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zl.lnxyls.cn

================================================================================
来源：http://pp.jctech888.com.cn

G. 面向对象
来源：http://hl.hahajie.cn

================================================================================
来源：http://op.yuntaijiaju.cn

[G01] 定义类
来源：http://wn.nicolike.cn

Py:   class User: pass
来源：http://ae.huixinmuqiang.cn

PHP:  class User {}
来源：http://ql.wgjwhj.cn

JS:   class User {}
来源：http://zg.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://it.9csxet.cn

Java: class User {}
来源：http://ra.huanxung.cn

Go:   type User struct { Name string }
来源：http://ck.lnxyls.cn

Ruby: class User; end
来源：http://bz.huixinmuqiang.cn

C#:   class User {}
来源：http://ib.chemitech.net.cn

[G02] 构造函数
来源：http://na.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://fx.muxihuayi.cn

PHP:  public function __construct(public string $name) {}
来源：http://oi.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://vw.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://ld.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://iv.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jx.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://cw.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://iq.huanxung.cn

[G03] 实例属性
来源：http://qn.wgjwhj.cn

Py:   self.name = "x"
来源：http://ka.521024.cn

PHP:  public string $name = "x";
来源：http://un.haigaiapp.cn

JS:   this.name = "x";
来源：http://dq.bookmarksfly.cn

TS:   name: string = "x";
来源：http://tp.bookmarksfly.cn

Java: private String name;
来源：http://jn.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cy.asd995.cn

Ruby: @name = "x"
来源：http://xs.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://lj.lnxyls.cn

[G04] 定义方法
来源：http://rf.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://th.szxytkj.cn


<!-- 参考信息 -->