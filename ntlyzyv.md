代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://jy.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zk.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ik.asd995.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ei.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://ls.szsharing.cn

[E07] 按分隔符拆分
来源：http://rd.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zj.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://io.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ux.newstarts.cn

TS:   s.split(",")
来源：http://rg.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ho.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xa.yuntaijiaju.cn

Ruby: s.split(",");  s.split
来源：http://nj.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ez.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://ms.haigaiapp.cn

Py:   ",".join(items)
来源：http://zo.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://bi.lnxyls.cn

JS:   items.join(",")
来源：http://zm.nszjky.cn

TS:   items.join(",")
来源：http://kn.wgjwhj.cn

Java: String.join(",", items)
来源：http://qr.colortex.cn

Go:   strings.Join(items, ",")
来源：http://bw.9csxet.cn

Ruby: items.join(",")
来源：http://nn.lnxyls.cn

C#:   string.Join(",", items)
来源：http://ue.lnxyls.cn

[E09] 去除所有空白字符
来源：http://cy.shxzukj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kv.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tu.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://tc.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://kv.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://ii.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yd.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mk.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zx.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://ui.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wp.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://my.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://pl.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://ty.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://vd.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dt.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yz.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zh.jctech888.com.cn

[E11] 反转字符串
来源：http://vz.yuexingan06.cn

Py:   s[::-1]
来源：http://gq.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://kl.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://tm.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://gt.huixiangedu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ht.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mb.colortex.cn

Ruby: s.reverse
来源：http://mt.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hb.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://nh.jianghongdianzi.cn

Py:   s.count("a")
来源：http://wr.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://mb.hahajie.cn

JS:   s.split("a").length - 1
来源：http://rt.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://yl.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zs.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://mp.haigaiapp.cn

Ruby: s.count("a")
来源：http://qa.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://wm.haigaiapp.cn

[E13] 逐字符遍历
来源：http://kb.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://lc.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kq.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pt.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gp.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ak.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dw.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zd.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ut.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://qq.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rm.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ut.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://il.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://if.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hy.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xf.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ph.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hg.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://lh.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rk.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kj.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aq.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gu.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ol.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jy.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pu.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hi.nicolike.cn

[E16] 数字千分位
来源：http://gy.huanxung.cn

Py:   f"{1234567:,}"
来源：http://ci.lnxyls.cn

PHP:  number_format(1234567);
来源：http://ha.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gl.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tn.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dz.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://do.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dt.colortex.cn

C#:   1234567.ToString("N0")
来源：http://jr.9csxet.cn

[E17] 首字母大写
来源：http://gm.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vy.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://id.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gq.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://io.nicolike.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pz.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kn.hahajie.cn

Ruby: s.capitalize
来源：http://za.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qk.shtwfgs.cn

[E18] 模板占位符替换
来源：http://um.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pk.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xo.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://js.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zs.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qh.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xr.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qp.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lc.huanxung.cn

[E19] 多行文本按行拆分
来源：http://ad.newstarts.cn

Py:   s.splitlines()
来源：http://cx.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://te.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://ee.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://wu.hahajie.cn

Java: s.lines().toList()
来源：http://is.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://hz.shxzukj.cn

Ruby: s.lines
来源：http://rw.newstarts.cn

C#:   s.Split('\n')
来源：http://ez.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://ej.huixiangedu.cn

Py:   if not s:
来源：http://hr.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sp.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bb.gzmigu.cn

TS:   if (s === "") {}
来源：http://kg.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://bh.hnjuh.cn

Go:   if s == "" {}
来源：http://pg.bjjhwx.cn

Ruby: if s.empty?
来源：http://ui.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ts.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://tg.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ym.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ml.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://on.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bg.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sa.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://gf.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sd.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ct.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://ns.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lq.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zv.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ic.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fz.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zd.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lw.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://lo.yuntaijiaju.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qc.panjiajie.cn

================================================================================
来源：http://vl.asd995.cn

F. 文件与目录
来源：http://yh.bookmarksfly.cn

================================================================================
来源：http://xg.muxihuayi.cn

[F01] 读取整个文件
来源：http://um.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bd.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://hb.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iu.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kg.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jm.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jg.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://mh.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://an.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://hp.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ra.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zb.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rd.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jk.szsharing.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vt.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dq.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://js.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fd.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://ib.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zd.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vr.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://us.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qv.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ge.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tt.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://df.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uk.szsharing.cn

[F04] 追加写入文件
来源：http://be.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://al.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fn.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ne.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ns.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://re.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tm.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://md.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jm.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://jo.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wd.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://kn.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://vj.jianghongdianzi.cn

TS:   fs.existsSync("a.txt")
来源：http://vv.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xo.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://on.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://ut.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://wp.huanxung.cn

[F06] 删除文件
来源：http://rh.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://eq.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://ab.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nm.szxytkj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://li.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ye.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://ie.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://bv.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://wd.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://eb.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rw.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ov.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qj.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qk.szxytkj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tm.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yg.hnjuh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jn.shtwfgs.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kl.huanxung.cn

[F08] 遍历目录
来源：http://mq.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ft.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vz.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://nc.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://wn.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hd.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zt.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://di.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://px.lnxyls.cn

[F09] 获取文件大小
来源：http://kj.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://ga.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://hy.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://ov.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://qd.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://et.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ql.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://mu.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://da.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://en.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pv.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oc.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sj.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://gu.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fg.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ys.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iq.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hq.muxihuayi.cn

[F11] 复制与移动文件
来源：http://hs.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jv.bjjhwx.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dw.bookmarksfly.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cf.newstarts.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ko.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lm.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kc.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sz.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rj.haigaiapp.cn

[F12] CSV 读写
来源：http://zk.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ju.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fn.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jl.yuntaijiaju.cn

TS:   // 同上
来源：http://qh.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ff.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dv.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mt.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sd.nicolike.cn

================================================================================
来源：http://sc.nszjky.cn

G. 面向对象
来源：http://md.szxytkj.cn

================================================================================
来源：http://jf.hnjuh.cn

[G01] 定义类
来源：http://pq.jianghongdianzi.cn

Py:   class User: pass
来源：http://uq.szsharing.cn

PHP:  class User {}
来源：http://jq.panjiajie.cn

JS:   class User {}
来源：http://qt.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://tb.gzmigu.cn

Java: class User {}
来源：http://ry.lnxyls.cn

Go:   type User struct { Name string }
来源：http://ba.haigaiapp.cn

Ruby: class User; end
来源：http://nk.nicolike.cn

C#:   class User {}
来源：http://fx.huixinmuqiang.cn

[G02] 构造函数
来源：http://bm.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://zu.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://eo.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ch.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://ap.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://ua.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gn.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://ia.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://zq.lnxyls.cn

[G03] 实例属性
来源：http://vj.szxytkj.cn

Py:   self.name = "x"
来源：http://gd.jianghongdianzi.cn

PHP:  public string $name = "x";
来源：http://fp.nicolike.cn

JS:   this.name = "x";
来源：http://xu.yuexingan06.cn

TS:   name: string = "x";
来源：http://bl.wgjwhj.cn

Java: private String name;
来源：http://jw.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vw.gzmigu.cn

Ruby: @name = "x"
来源：http://ym.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://hp.jianghongdianzi.cn

[G04] 定义方法
来源：http://xl.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://wk.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yg.szsharing.cn

JS:   greet() { return this.name; }
来源：http://nz.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://ti.muxihuayi.cn

Java: String greet() { return name; }
来源：http://xh.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vk.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://ij.nicolike.cn

C#:   public string Greet() => Name;
来源：http://so.hahajie.cn

[G05] 继承
来源：http://ts.haigaiapp.cn


<!-- 参考信息 -->