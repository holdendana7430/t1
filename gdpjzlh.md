代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://qo.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mu.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iw.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yy.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://fx.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://ry.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zi.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tg.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://eh.lnxyls.cn

TS:   s.split(",")
来源：http://yd.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kf.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mf.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://jl.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dk.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://ng.colortex.cn

Py:   ",".join(items)
来源：http://qx.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://xi.jianghongdianzi.cn

JS:   items.join(",")
来源：http://ih.yuexingan06.cn

TS:   items.join(",")
来源：http://pv.szxytkj.cn

Java: String.join(",", items)
来源：http://dn.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://ly.hahajie.cn

Ruby: items.join(",")
来源：http://jl.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://js.hnjuh.cn

[E09] 去除所有空白字符
来源：http://wl.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bx.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xt.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://cy.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://il.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://rp.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qx.huixinmuqiang.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dn.huixiangedu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mr.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://fk.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yx.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ni.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://aa.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://py.szsharing.cn

Java: String.format("%03d", 7)
来源：http://ko.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xy.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vy.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://te.shxzukj.cn

[E11] 反转字符串
来源：http://rs.yuntaijiaju.cn

Py:   s[::-1]
来源：http://rn.wgjwhj.cn

PHP:  strrev($s);
来源：http://er.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://yx.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://gi.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jj.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ln.shtwfgs.cn

Ruby: s.reverse
来源：http://an.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tz.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://pq.newstarts.cn

Py:   s.count("a")
来源：http://oh.wgjwhj.cn

PHP:  substr_count($s, "a");
来源：http://no.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://uw.nszjky.cn

TS:   s.split("a").length - 1
来源：http://rz.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pk.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://am.hahajie.cn

Ruby: s.count("a")
来源：http://ox.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://fc.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://el.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://yo.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dj.bjjhwx.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wi.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jg.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mk.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ne.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nb.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ys.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://ww.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zk.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ci.asd995.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zd.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eg.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://df.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mx.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ta.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ti.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://bp.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xw.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ez.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dx.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tt.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sp.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ck.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://of.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cg.wgjwhj.cn

[E16] 数字千分位
来源：http://gu.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://gt.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://fq.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gm.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sz.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pp.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ho.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ov.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://kj.521024.cn

[E17] 首字母大写
来源：http://ik.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wb.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://na.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xb.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ra.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rg.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xz.bookmarksfly.cn

Ruby: s.capitalize
来源：http://ss.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tt.wgjwhj.cn

[E18] 模板占位符替换
来源：http://uo.9csxet.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uf.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://so.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://oi.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nn.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tp.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ct.newstarts.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sa.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fe.nszjky.cn

[E19] 多行文本按行拆分
来源：http://ox.panjiajie.cn

Py:   s.splitlines()
来源：http://zp.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xa.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://un.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://ud.jctech888.com.cn

Java: s.lines().toList()
来源：http://yz.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://ej.shxzskj.cn

Ruby: s.lines
来源：http://ww.asd995.cn

C#:   s.Split('\n')
来源：http://bf.nszjky.cn

[E20] 判断字符串是否为空
来源：http://cl.wgjwhj.cn

Py:   if not s:
来源：http://xq.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hd.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mi.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://qy.521024.cn

Java: if (s.isEmpty()) {}
来源：http://ig.shxzukj.cn

Go:   if s == "" {}
来源：http://cf.colortex.cn

Ruby: if s.empty?
来源：http://jw.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bv.9csxet.cn

[E21] 超长截断加省略号
来源：http://io.shxzukj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lk.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qr.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ql.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dj.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gj.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://ol.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wd.asd995.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kq.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://ub.shxzukj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lb.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pb.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kn.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gh.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yj.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vp.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://sy.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ss.9csxet.cn

================================================================================
来源：http://ba.jianghongdianzi.cn

F. 文件与目录
来源：http://lg.huixinmuqiang.cn

================================================================================
来源：http://hy.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://vq.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ek.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://di.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ly.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sg.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fx.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rb.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://tx.panjiajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://mr.521024.cn

[F02] 逐行读取文件
来源：http://lp.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fj.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ry.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://es.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lb.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://we.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tg.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sa.nszjky.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://by.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://wu.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nr.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lb.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wu.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mi.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ki.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ib.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://vz.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ge.panjiajie.cn

[F04] 追加写入文件
来源：http://yy.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ap.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zd.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gc.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aa.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dc.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ph.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gu.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vu.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://re.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vp.colortex.cn

PHP:  file_exists("a.txt");
来源：http://uw.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://tq.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://jj.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pa.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fv.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://tf.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://ic.huixiangedu.cn

[F06] 删除文件
来源：http://or.wgjwhj.cn

Py:   os.remove("a.txt")
来源：http://ix.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://pe.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ga.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ob.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xk.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://go.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://vp.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://bn.nszjky.cn

[F07] 创建目录（含多级）
来源：http://jt.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sm.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gq.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zr.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ud.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jy.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zh.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oh.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nj.shxzskj.cn

[F08] 遍历目录
来源：http://mp.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ma.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yt.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://op.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://cd.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dn.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ak.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://mv.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://gt.shxzskj.cn

[F09] 获取文件大小
来源：http://zd.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://ws.newstarts.cn

PHP:  filesize("a.txt");
来源：http://uo.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://qj.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://oi.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nd.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mz.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://rk.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://qx.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://fo.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://in.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nn.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uo.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://dr.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mg.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uh.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kh.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xl.haigaiapp.cn

[F11] 复制与移动文件
来源：http://ne.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vu.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zo.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bi.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bo.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fn.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mg.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://be.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zg.shtwfgs.cn

[F12] CSV 读写
来源：http://wh.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qu.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mq.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://go.huixinmuqiang.cn

TS:   // 同上
来源：http://sx.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iw.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xy.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pr.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dx.panjiajie.cn

================================================================================
来源：http://se.yuexingan06.cn

G. 面向对象
来源：http://ny.yuntaijiaju.cn

================================================================================
来源：http://db.huixinmuqiang.cn

[G01] 定义类
来源：http://xs.huanxung.cn

Py:   class User: pass
来源：http://om.hnjuh.cn

PHP:  class User {}
来源：http://jq.muxihuayi.cn

JS:   class User {}
来源：http://tv.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://qx.asd995.cn

Java: class User {}
来源：http://tr.asd995.cn

Go:   type User struct { Name string }
来源：http://bu.lnxyls.cn

Ruby: class User; end
来源：http://sv.newstarts.cn

C#:   class User {}
来源：http://mx.9csxet.cn

[G02] 构造函数
来源：http://jp.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://zh.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://jp.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://qd.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://pz.521024.cn

Java: User(String name) { this.name = name; }
来源：http://yh.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eh.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://gc.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://ln.huanxung.cn

[G03] 实例属性
来源：http://zx.lnxyls.cn

Py:   self.name = "x"
来源：http://ua.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://uw.yuexingan06.cn

JS:   this.name = "x";
来源：http://yz.newstarts.cn

TS:   name: string = "x";
来源：http://vd.nszjky.cn

Java: private String name;
来源：http://wc.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kq.9csxet.cn

Ruby: @name = "x"
来源：http://zj.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://ky.9csxet.cn

[G04] 定义方法
来源：http://kf.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://eg.huixinmuqiang.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nd.nicolike.cn

JS:   greet() { return this.name; }
来源：http://xc.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://yv.newstarts.cn

Java: String greet() { return name; }
来源：http://rq.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vj.nszjky.cn

Ruby: def greet; @name; end
来源：http://cl.szsharing.cn

C#:   public string Greet() => Name;
来源：http://nb.nicolike.cn

[G05] 继承
来源：http://ep.hahajie.cn


<!-- 参考信息 -->