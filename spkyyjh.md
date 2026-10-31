代发 wailian999

C#:   s.Replace("a", "b")
来源：http://tr.hnjuh.cn

[E07] 按分隔符拆分
来源：http://gf.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://co.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dd.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.colortex.cn

TS:   s.split(",")
来源：http://ac.szxytkj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qi.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ik.yuntaijiaju.cn

Ruby: s.split(",");  s.split
来源：http://xf.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iz.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://um.asd995.cn

Py:   ",".join(items)
来源：http://sb.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://og.bookmarksfly.cn

JS:   items.join(",")
来源：http://jk.newstarts.cn

TS:   items.join(",")
来源：http://mq.muxihuayi.cn

Java: String.join(",", items)
来源：http://qe.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://kx.shxzskj.cn

Ruby: items.join(",")
来源：http://pp.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://kt.nszjky.cn

[E09] 去除所有空白字符
来源：http://ta.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iy.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://na.hahajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://mq.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://tp.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://gi.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://da.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://te.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lg.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://sc.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sa.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cc.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://sr.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://jy.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://si.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lj.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xc.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xg.colortex.cn

[E11] 反转字符串
来源：http://mq.shtwfgs.cn

Py:   s[::-1]
来源：http://qw.nicolike.cn

PHP:  strrev($s);
来源：http://xy.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://xc.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://kr.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://eb.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ko.gzmigu.cn

Ruby: s.reverse
来源：http://rb.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hs.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://hg.newstarts.cn

Py:   s.count("a")
来源：http://va.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://fa.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://ch.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://wm.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hp.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://dl.colortex.cn

Ruby: s.count("a")
来源：http://lv.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://df.9csxet.cn

[E13] 逐字符遍历
来源：http://ho.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://nr.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bm.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://op.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sw.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pg.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pi.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cs.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nd.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://rl.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://la.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mo.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sn.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ej.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ho.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uf.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://an.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oo.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://dh.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://le.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ww.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zi.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xl.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xc.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qu.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vc.hahajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ol.muxihuayi.cn

[E16] 数字千分位
来源：http://zr.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://ol.521024.cn

PHP:  number_format(1234567);
来源：http://rh.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tb.jianghongdianzi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ic.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fi.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hr.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cr.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://sq.colortex.cn

[E17] 首字母大写
来源：http://zy.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://me.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ll.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nu.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yb.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sd.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qx.lnxyls.cn

Ruby: s.capitalize
来源：http://rf.huixinmuqiang.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lh.muxihuayi.cn

[E18] 模板占位符替换
来源：http://zh.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oo.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tk.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mi.lnxyls.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dh.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gx.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yv.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pc.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://en.521024.cn

[E19] 多行文本按行拆分
来源：http://tj.521024.cn

Py:   s.splitlines()
来源：http://uu.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vk.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://um.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://qx.nicolike.cn

Java: s.lines().toList()
来源：http://dq.521024.cn

Go:   strings.Split(s, "\n")
来源：http://kv.chemitech.net.cn

Ruby: s.lines
来源：http://ew.521024.cn

C#:   s.Split('\n')
来源：http://op.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://zi.colortex.cn

Py:   if not s:
来源：http://zn.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tx.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ww.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://vq.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://om.yuexingan06.cn

Go:   if s == "" {}
来源：http://bt.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://ab.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iu.521024.cn

[E21] 超长截断加省略号
来源：http://ds.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ev.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://az.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dw.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wk.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ox.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://tb.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xc.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tp.9csxet.cn

[E22] 字节长度与字符长度
来源：http://jk.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uw.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ma.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fc.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ja.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sq.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pp.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://xa.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yw.bjjhwx.cn

================================================================================
来源：http://mw.jctech888.com.cn

F. 文件与目录
来源：http://ie.shxzukj.cn

================================================================================
来源：http://fo.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://wv.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uj.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://sg.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eb.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dd.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sy.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://af.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://uw.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://kg.szxytkj.cn

[F02] 逐行读取文件
来源：http://ms.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://va.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fj.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kw.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mq.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mm.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hq.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fu.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://un.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://gy.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iy.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nw.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://de.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iq.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bw.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tn.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://nn.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ra.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://hr.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ne.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dw.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ko.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ef.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://py.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cx.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://di.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ge.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://ce.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aj.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://gz.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://ua.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://lv.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yn.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qx.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://cz.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://oo.asd995.cn

[F06] 删除文件
来源：http://so.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://ig.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://mk.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wq.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wb.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xy.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://vx.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://at.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://qo.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://nm.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pw.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rs.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zf.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cc.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nu.521024.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aj.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sj.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ld.hahajie.cn

[F08] 遍历目录
来源：http://aw.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yb.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rl.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://jp.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://fs.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ul.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qj.shxzskj.cn

Ruby: Dir.children("dir")
来源：http://xf.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://xf.huanxung.cn

[F09] 获取文件大小
来源：http://ii.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://af.521024.cn

PHP:  filesize("a.txt");
来源：http://qg.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://ky.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://co.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://me.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hv.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://pj.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://ml.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://bd.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sp.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ig.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tq.colortex.cn

TS:   path.extname("a.txt")
来源：http://nk.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cq.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ei.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ck.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qy.nicolike.cn

[F11] 复制与移动文件
来源：http://ha.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vs.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://br.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wt.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mr.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rp.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ne.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xc.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ms.521024.cn

[F12] CSV 读写
来源：http://iy.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hs.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ut.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ap.colortex.cn

TS:   // 同上
来源：http://kp.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wh.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qg.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wy.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fv.huixiangedu.cn

================================================================================
来源：http://rj.asd995.cn

G. 面向对象
来源：http://sw.9csxet.cn

================================================================================
来源：http://bg.jctech888.com.cn

[G01] 定义类
来源：http://nx.yuntaijiaju.cn

Py:   class User: pass
来源：http://tu.hnjuh.cn

PHP:  class User {}
来源：http://qf.nszjky.cn

JS:   class User {}
来源：http://bh.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://oe.colortex.cn

Java: class User {}
来源：http://rj.newstarts.cn

Go:   type User struct { Name string }
来源：http://sr.huixiangedu.cn

Ruby: class User; end
来源：http://en.huixinmuqiang.cn

C#:   class User {}
来源：http://ik.gzmigu.cn

[G02] 构造函数
来源：http://kd.szxytkj.cn

Py:   def __init__(self, name): self.name = name
来源：http://qe.muxihuayi.cn

PHP:  public function __construct(public string $name) {}
来源：http://oj.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://kw.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://oh.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://ed.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bx.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://ov.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://jq.jianghongdianzi.cn

[G03] 实例属性
来源：http://jx.muxihuayi.cn

Py:   self.name = "x"
来源：http://vw.nszjky.cn

PHP:  public string $name = "x";
来源：http://aa.bookmarksfly.cn

JS:   this.name = "x";
来源：http://lr.521024.cn

TS:   name: string = "x";
来源：http://ls.9csxet.cn

Java: private String name;
来源：http://sl.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mw.muxihuayi.cn

Ruby: @name = "x"
来源：http://hb.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://ph.521024.cn

[G04] 定义方法
来源：http://ag.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://wn.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oq.huanxung.cn

JS:   greet() { return this.name; }
来源：http://fb.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://bu.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://vi.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ut.lnxyls.cn

Ruby: def greet; @name; end
来源：http://un.colortex.cn

C#:   public string Greet() => Name;
来源：http://th.muxihuayi.cn

[G05] 继承
来源：http://rc.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://zb.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://wa.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://wa.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://pn.hahajie.cn


<!-- 参考信息 -->