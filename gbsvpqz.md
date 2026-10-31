代发 wailian999

PHP:  implode(",", $items);
来源：http://er.asd995.cn

JS:   items.join(",")
来源：http://av.bjjhwx.cn

TS:   items.join(",")
来源：http://sr.szsharing.cn

Java: String.join(",", items)
来源：http://ah.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://eh.huixiangedu.cn

Ruby: items.join(",")
来源：http://ia.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://ck.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://vr.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gj.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://er.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://cu.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://iw.jianghongdianzi.cn

Java: s.replaceAll("\\s+", "")
来源：http://od.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xz.bookmarksfly.cn

Ruby: s.gsub(/\s+/, "")
来源：http://os.szsharing.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qa.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://js.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hm.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fj.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://mc.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://cc.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://fn.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uy.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mq.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ee.nszjky.cn

[E11] 反转字符串
来源：http://fj.shtwfgs.cn

Py:   s[::-1]
来源：http://nu.shtwfgs.cn

PHP:  strrev($s);
来源：http://ek.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://dj.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://tf.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://or.yuexingan06.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lv.bookmarksfly.cn

Ruby: s.reverse
来源：http://xe.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ix.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://ek.muxihuayi.cn

Py:   s.count("a")
来源：http://hq.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://nn.521024.cn

JS:   s.split("a").length - 1
来源：http://iw.521024.cn

TS:   s.split("a").length - 1
来源：http://dm.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xt.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://dw.huanxung.cn

Ruby: s.count("a")
来源：http://en.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://as.shxzukj.cn

[E13] 逐字符遍历
来源：http://gf.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://uc.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fv.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xc.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jj.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gp.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zv.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uv.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yk.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://ei.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ll.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vk.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iu.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tx.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fh.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nd.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ef.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ut.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://ko.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bn.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lw.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qm.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bn.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bs.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ms.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qd.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bz.bjjhwx.cn

[E16] 数字千分位
来源：http://ve.yuexingan06.cn

Py:   f"{1234567:,}"
来源：http://vq.hahajie.cn

PHP:  number_format(1234567);
来源：http://fu.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fr.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://or.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://no.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dr.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bz.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://eu.bookmarksfly.cn

[E17] 首字母大写
来源：http://me.nszjky.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fr.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fd.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cg.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://us.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://io.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gg.521024.cn

Ruby: s.capitalize
来源：http://wl.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jb.chemitech.net.cn

[E18] 模板占位符替换
来源：http://mo.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://te.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xs.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://oz.asd995.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nb.gzmigu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hp.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iw.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gr.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gi.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://fg.chemitech.net.cn

Py:   s.splitlines()
来源：http://qy.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dy.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://xw.521024.cn

TS:   s.split(/\r?\n/)
来源：http://yb.muxihuayi.cn

Java: s.lines().toList()
来源：http://qm.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://jb.huanxung.cn

Ruby: s.lines
来源：http://ho.colortex.cn

C#:   s.Split('\n')
来源：http://ia.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://rm.huanxung.cn

Py:   if not s:
来源：http://oe.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gt.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oa.colortex.cn

TS:   if (s === "") {}
来源：http://cs.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://tu.huixiangedu.cn

Go:   if s == "" {}
来源：http://yf.huanxung.cn

Ruby: if s.empty?
来源：http://oj.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oq.newstarts.cn

[E21] 超长截断加省略号
来源：http://ja.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tw.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kw.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wk.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pa.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kq.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://bd.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ip.asd995.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hk.521024.cn

[E22] 字节长度与字符长度
来源：http://ue.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bt.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rt.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ma.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yf.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yu.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://py.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://ab.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dr.bookmarksfly.cn

================================================================================
来源：http://dj.bjjhwx.cn

F. 文件与目录
来源：http://kf.nszjky.cn

================================================================================
来源：http://ds.521024.cn

[F01] 读取整个文件
来源：http://nd.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iz.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://cp.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wa.muxihuayi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yn.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ob.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ux.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://gr.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://jn.haigaiapp.cn

[F02] 逐行读取文件
来源：http://oj.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pa.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://as.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ni.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kz.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nm.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://su.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ok.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wi.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://ra.lnxyls.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dq.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vx.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xu.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fp.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fh.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ve.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://dg.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://at.muxihuayi.cn

[F04] 追加写入文件
来源：http://qj.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zf.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yf.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vy.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ae.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sf.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ac.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vq.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ol.nicolike.cn

[F05] 判断文件或目录是否存在
来源：http://fe.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xj.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://kf.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://uj.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://lu.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kj.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yd.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://zx.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://ob.huixinmuqiang.cn

[F06] 删除文件
来源：http://cu.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://yy.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://fs.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hs.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wf.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hj.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://av.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://gg.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://rr.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://bb.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ys.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oa.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://df.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mh.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vo.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lj.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zq.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ck.wgjwhj.cn

[F08] 遍历目录
来源：http://xa.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vt.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://su.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://zh.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://zn.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sh.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ch.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://no.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://go.szsharing.cn

[F09] 获取文件大小
来源：http://lj.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://kh.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://sz.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://fe.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://nn.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rd.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://py.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://as.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://jq.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://qt.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ec.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ku.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mk.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://mw.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hk.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yn.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hd.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hi.lnxyls.cn

[F11] 复制与移动文件
来源：http://md.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ae.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nx.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zk.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kx.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dh.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://je.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xe.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jk.9csxet.cn

[F12] CSV 读写
来源：http://ap.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dc.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ud.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://im.jianghongdianzi.cn

TS:   // 同上
来源：http://rw.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rc.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rv.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zb.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ej.asd995.cn

================================================================================
来源：http://rd.yuexingan06.cn

G. 面向对象
来源：http://gl.hahajie.cn

================================================================================
来源：http://qd.szxytkj.cn

[G01] 定义类
来源：http://kj.wgjwhj.cn

Py:   class User: pass
来源：http://qw.huixinmuqiang.cn

PHP:  class User {}
来源：http://gi.hnjuh.cn

JS:   class User {}
来源：http://qv.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://qj.yuexingan06.cn

Java: class User {}
来源：http://jn.hnjuh.cn

Go:   type User struct { Name string }
来源：http://wg.9csxet.cn

Ruby: class User; end
来源：http://dy.jianghongdianzi.cn

C#:   class User {}
来源：http://bk.szxytkj.cn

[G02] 构造函数
来源：http://ny.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://ja.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://qp.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://wq.521024.cn

TS:   constructor(public name: string) {}
来源：http://fs.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://gx.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bz.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://sq.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://il.521024.cn

[G03] 实例属性
来源：http://kz.shxzukj.cn

Py:   self.name = "x"
来源：http://lw.huanxung.cn

PHP:  public string $name = "x";
来源：http://dy.9csxet.cn

JS:   this.name = "x";
来源：http://pg.colortex.cn

TS:   name: string = "x";
来源：http://rz.asd995.cn

Java: private String name;
来源：http://pv.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zy.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://yt.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://df.bookmarksfly.cn

[G04] 定义方法
来源：http://wi.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://vp.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ut.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://ju.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://fz.newstarts.cn

Java: String greet() { return name; }
来源：http://kp.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rr.9csxet.cn

Ruby: def greet; @name; end
来源：http://gy.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://yd.hahajie.cn

[G05] 继承
来源：http://bt.shxzskj.cn

Py:   class Admin(User): pass
来源：http://ow.nicolike.cn

PHP:  class Admin extends User {}
来源：http://sh.szxytkj.cn

JS:   class Admin extends User {}
来源：http://ac.asd995.cn

TS:   class Admin extends User {}
来源：http://dw.9csxet.cn

Java: class Admin extends User {}
来源：http://lh.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ml.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://ei.shtwfgs.cn

C#:   class Admin : User {}
来源：http://tn.gzmigu.cn

[G06] 重写方法
来源：http://nc.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://si.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sx.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://mj.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://gl.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://xl.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ey.521024.cn

Ruby: def greet; "admin"; end
来源：http://ou.asd995.cn


<!-- 参考信息 -->