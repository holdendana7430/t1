代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://zw.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oe.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ce.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mu.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://ag.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://ye.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bw.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ke.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oz.newstarts.cn

TS:   s.split(",")
来源：http://ys.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kk.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gh.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://jk.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sq.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://zf.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://co.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://yb.hnjuh.cn

JS:   items.join(",")
来源：http://lw.nszjky.cn

TS:   items.join(",")
来源：http://dl.huixiangedu.cn

Java: String.join(",", items)
来源：http://gc.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://zt.nicolike.cn

Ruby: items.join(",")
来源：http://mc.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://sr.shxzukj.cn

[E09] 去除所有空白字符
来源：http://hx.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wc.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ov.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://rq.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://zs.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://ct.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://iu.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://za.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lz.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://pm.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kb.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://io.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://iy.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://us.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://ql.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pb.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qj.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wk.nszjky.cn

[E11] 反转字符串
来源：http://xu.521024.cn

Py:   s[::-1]
来源：http://ky.szsharing.cn

PHP:  strrev($s);
来源：http://to.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://ya.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://oj.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sp.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pa.9csxet.cn

Ruby: s.reverse
来源：http://jx.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rn.521024.cn

[E12] 统计某字符出现次数
来源：http://cv.hnjuh.cn

Py:   s.count("a")
来源：http://zb.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://yl.nszjky.cn

JS:   s.split("a").length - 1
来源：http://aa.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://dg.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ic.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://hn.hahajie.cn

Ruby: s.count("a")
来源：http://rq.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://ur.chemitech.net.cn

[E13] 逐字符遍历
来源：http://rt.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://ql.bjjhwx.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sm.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lk.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ey.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yg.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vy.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ek.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nl.9csxet.cn

[E14] URL 编码与 Base64
来源：http://kt.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xq.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pl.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ws.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nn.nszjky.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yq.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jv.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wu.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fj.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://ub.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hj.haigaiapp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gi.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vs.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eu.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cy.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jc.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mi.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ti.lnxyls.cn

[E16] 数字千分位
来源：http://xn.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://mt.shxzskj.cn

PHP:  number_format(1234567);
来源：http://rb.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xh.panjiajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hc.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://at.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pl.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://og.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://fa.muxihuayi.cn

[E17] 首字母大写
来源：http://gw.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xj.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dd.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tl.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://si.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kc.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dr.muxihuayi.cn

Ruby: s.capitalize
来源：http://mb.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://he.shxzskj.cn

[E18] 模板占位符替换
来源：http://rd.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bo.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uf.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cw.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cx.yuexingan06.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mc.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sb.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lu.nszjky.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fd.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://gs.521024.cn

Py:   s.splitlines()
来源：http://go.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dt.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://xt.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://gy.asd995.cn

Java: s.lines().toList()
来源：http://ox.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://aa.wgjwhj.cn

Ruby: s.lines
来源：http://bw.szsharing.cn

C#:   s.Split('\n')
来源：http://ax.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://yl.jctech888.com.cn

Py:   if not s:
来源：http://kb.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rp.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pg.jctech888.com.cn

TS:   if (s === "") {}
来源：http://yx.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://jm.huanxung.cn

Go:   if s == "" {}
来源：http://km.panjiajie.cn

Ruby: if s.empty?
来源：http://km.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://of.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://md.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bu.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cn.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gc.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ef.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gm.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://db.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cc.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ar.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://js.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pt.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ik.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cz.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ip.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tr.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pv.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://go.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tr.newstarts.cn

================================================================================
来源：http://vz.bjjhwx.cn

F. 文件与目录
来源：http://ln.nszjky.cn

================================================================================
来源：http://aw.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://dy.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ca.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://fw.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kg.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ts.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ry.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ce.nicolike.cn

Ruby: File.read("a.txt")
来源：http://lh.asd995.cn

C#:   File.ReadAllText("a.txt");
来源：http://zz.szxytkj.cn

[F02] 逐行读取文件
来源：http://nb.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://py.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://au.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tq.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ez.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tk.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mq.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uv.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vy.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://rj.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dl.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tl.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kx.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ja.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dy.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dg.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://dg.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wm.shxzukj.cn

[F04] 追加写入文件
来源：http://zr.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://da.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zd.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://af.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hx.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jw.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cl.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://md.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yq.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://wn.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ww.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://vi.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://vf.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://hv.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lq.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kd.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://ul.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://cu.asd995.cn

[F06] 删除文件
来源：http://ev.newstarts.cn

Py:   os.remove("a.txt")
来源：http://ge.521024.cn

PHP:  unlink("a.txt");
来源：http://zu.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rm.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gj.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rh.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://sn.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://bx.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://gm.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://xu.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mn.panjiajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://el.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jr.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mc.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xm.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yh.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://op.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kv.jctech888.com.cn

[F08] 遍历目录
来源：http://lc.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kp.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cx.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://px.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://by.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rz.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yd.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://qj.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://md.hahajie.cn

[F09] 获取文件大小
来源：http://ir.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://wv.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://zr.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://ur.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://ua.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ry.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mq.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://en.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://ce.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://kk.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yx.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fg.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ni.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://dn.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vu.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ri.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dw.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xx.521024.cn

[F11] 复制与移动文件
来源：http://tf.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sh.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://si.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vb.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ue.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hg.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ii.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ej.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qy.lnxyls.cn

[F12] CSV 读写
来源：http://us.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cj.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fo.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bf.521024.cn

TS:   // 同上
来源：http://ac.yuntaijiaju.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bv.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ib.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jw.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ni.lnxyls.cn

================================================================================
来源：http://pb.bookmarksfly.cn

G. 面向对象
来源：http://ut.szxytkj.cn

================================================================================
来源：http://mb.hahajie.cn

[G01] 定义类
来源：http://op.hnjuh.cn

Py:   class User: pass
来源：http://va.panjiajie.cn

PHP:  class User {}
来源：http://lb.huixiangedu.cn

JS:   class User {}
来源：http://fe.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://zd.huixiangedu.cn

Java: class User {}
来源：http://co.lnxyls.cn

Go:   type User struct { Name string }
来源：http://cx.newstarts.cn

Ruby: class User; end
来源：http://cg.shxzskj.cn

C#:   class User {}
来源：http://rk.szxytkj.cn

[G02] 构造函数
来源：http://fb.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://of.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://mq.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://zh.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://tb.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://fq.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tn.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://ge.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://wi.haigaiapp.cn

[G03] 实例属性
来源：http://uo.9csxet.cn

Py:   self.name = "x"
来源：http://sw.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://hw.newstarts.cn

JS:   this.name = "x";
来源：http://fk.nicolike.cn

TS:   name: string = "x";
来源：http://ek.shxzukj.cn

Java: private String name;
来源：http://ab.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yt.bookmarksfly.cn

Ruby: @name = "x"
来源：http://zd.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://zv.huanxung.cn

[G04] 定义方法
来源：http://uf.szsharing.cn

Py:   def greet(self): return self.name
来源：http://po.huixinmuqiang.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hd.9csxet.cn

JS:   greet() { return this.name; }
来源：http://ob.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://bp.szxytkj.cn

Java: String greet() { return name; }
来源：http://fr.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zu.colortex.cn

Ruby: def greet; @name; end
来源：http://gq.szsharing.cn

C#:   public string Greet() => Name;
来源：http://ch.shxzukj.cn

[G05] 继承
来源：http://kf.shxzskj.cn


<!-- 参考信息 -->