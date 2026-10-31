代发 wailian999

PHP:  implode(",", $items);
来源：http://jt.lnxyls.cn

JS:   items.join(",")
来源：http://th.shxzukj.cn

TS:   items.join(",")
来源：http://tc.szxytkj.cn

Java: String.join(",", items)
来源：http://ji.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://tf.hahajie.cn

Ruby: items.join(",")
来源：http://gj.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://ct.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://rf.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bm.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nq.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://rc.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://xo.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://gb.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ya.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qc.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bh.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://oh.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zu.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kn.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://ju.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://am.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://yi.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bp.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jg.yuexingan06.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fq.shtwfgs.cn

[E11] 反转字符串
来源：http://yg.shtwfgs.cn

Py:   s[::-1]
来源：http://ob.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://qa.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://cv.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://ux.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jj.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://na.panjiajie.cn

Ruby: s.reverse
来源：http://ij.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nm.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://up.9csxet.cn

Py:   s.count("a")
来源：http://xu.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://jc.nicolike.cn

JS:   s.split("a").length - 1
来源：http://aw.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://fa.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qc.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://hg.jctech888.com.cn

Ruby: s.count("a")
来源：http://fb.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://gs.haigaiapp.cn

[E13] 逐字符遍历
来源：http://fv.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://ff.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fs.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gd.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uk.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zp.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hn.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jv.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ud.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://cg.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ds.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://br.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://im.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sj.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hy.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cu.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vi.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ne.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://yd.muxihuayi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ms.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yd.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mv.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nm.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oh.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cp.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xy.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gv.yuexingan06.cn

[E16] 数字千分位
来源：http://oq.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://im.szsharing.cn

PHP:  number_format(1234567);
来源：http://vy.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lt.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ux.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ey.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cy.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gh.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://lw.huixinmuqiang.cn

[E17] 首字母大写
来源：http://ck.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cc.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hc.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ux.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kw.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://da.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hr.gzmigu.cn

Ruby: s.capitalize
来源：http://fd.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sx.szsharing.cn

[E18] 模板占位符替换
来源：http://fa.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ri.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qi.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rp.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://us.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ks.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jk.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zp.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yd.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://oy.bjjhwx.cn

Py:   s.splitlines()
来源：http://xu.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lb.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://eq.huixiangedu.cn

TS:   s.split(/\r?\n/)
来源：http://lq.lnxyls.cn

Java: s.lines().toList()
来源：http://ha.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://xy.asd995.cn

Ruby: s.lines
来源：http://io.yuexingan06.cn

C#:   s.Split('\n')
来源：http://kc.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://qr.bookmarksfly.cn

Py:   if not s:
来源：http://ub.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://av.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ji.yuexingan06.cn

TS:   if (s === "") {}
来源：http://bf.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://sq.hahajie.cn

Go:   if s == "" {}
来源：http://tx.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://zx.9csxet.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cq.nszjky.cn

[E21] 超长截断加省略号
来源：http://hf.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lb.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cj.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ao.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bf.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ql.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://er.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yw.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pp.nszjky.cn

[E22] 字节长度与字符长度
来源：http://vd.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fr.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gl.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://il.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gb.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yd.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qh.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://uc.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dt.szsharing.cn

================================================================================
来源：http://nq.huanxung.cn

F. 文件与目录
来源：http://ap.chemitech.net.cn

================================================================================
来源：http://cq.szsharing.cn

[F01] 读取整个文件
来源：http://pd.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hf.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://ci.chemitech.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ef.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kl.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hb.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xy.hahajie.cn

Ruby: File.read("a.txt")
来源：http://qv.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://hc.colortex.cn

[F02] 逐行读取文件
来源：http://wc.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rc.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tl.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lu.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://un.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yt.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qy.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gw.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ic.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://cv.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fm.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://by.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rk.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xn.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kt.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://er.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://qe.lnxyls.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lv.shtwfgs.cn

[F04] 追加写入文件
来源：http://qy.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lc.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wx.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wx.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ae.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ma.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lr.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tq.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iu.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://re.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zf.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://zb.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://th.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://zn.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://if.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://su.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://ut.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://du.jianghongdianzi.cn

[F06] 删除文件
来源：http://wz.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://jj.521024.cn

PHP:  unlink("a.txt");
来源：http://gn.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://db.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ub.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://az.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://yg.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://jk.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://ki.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://ci.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pd.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pe.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uy.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vd.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xy.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://iu.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tf.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fw.bjjhwx.cn

[F08] 遍历目录
来源：http://jt.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://al.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iq.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://cp.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://fz.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://va.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hl.shxzskj.cn

Ruby: Dir.children("dir")
来源：http://yk.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://ew.haigaiapp.cn

[F09] 获取文件大小
来源：http://ys.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://cp.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://ri.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://ud.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://ha.521024.cn

Java: Files.size(Path.of("a.txt"))
来源：http://go.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vl.colortex.cn

Ruby: File.size("a.txt")
来源：http://fl.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://sr.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://nm.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dc.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bz.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bv.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://yd.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://of.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tn.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gg.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ip.bjjhwx.cn

[F11] 复制与移动文件
来源：http://ju.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lp.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ej.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vz.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sl.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hl.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gp.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pp.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://te.huanxung.cn

[F12] CSV 读写
来源：http://ye.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://va.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cv.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jt.newstarts.cn

TS:   // 同上
来源：http://lo.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oi.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ap.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ca.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gc.yuntaijiaju.cn

================================================================================
来源：http://zy.yuexingan06.cn

G. 面向对象
来源：http://ym.yuexingan06.cn

================================================================================
来源：http://gm.jianghongdianzi.cn

[G01] 定义类
来源：http://vw.asd995.cn

Py:   class User: pass
来源：http://eh.shxzukj.cn

PHP:  class User {}
来源：http://qh.muxihuayi.cn

JS:   class User {}
来源：http://zx.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://fr.szxytkj.cn

Java: class User {}
来源：http://it.hnjuh.cn

Go:   type User struct { Name string }
来源：http://og.9csxet.cn

Ruby: class User; end
来源：http://qk.shxzskj.cn

C#:   class User {}
来源：http://df.huanxung.cn

[G02] 构造函数
来源：http://sq.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://vt.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://ok.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://yn.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://la.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://du.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qu.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://bc.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://bo.gzmigu.cn

[G03] 实例属性
来源：http://hb.gzmigu.cn

Py:   self.name = "x"
来源：http://xl.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://db.muxihuayi.cn

JS:   this.name = "x";
来源：http://pl.521024.cn

TS:   name: string = "x";
来源：http://lt.bjjhwx.cn

Java: private String name;
来源：http://nu.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oj.szxytkj.cn

Ruby: @name = "x"
来源：http://td.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://nj.shxzukj.cn

[G04] 定义方法
来源：http://pk.huanxung.cn

Py:   def greet(self): return self.name
来源：http://ho.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://va.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://kp.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://tm.asd995.cn

Java: String greet() { return name; }
来源：http://rz.jianghongdianzi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tm.shxzskj.cn

Ruby: def greet; @name; end
来源：http://gn.9csxet.cn

C#:   public string Greet() => Name;
来源：http://bn.szsharing.cn

[G05] 继承
来源：http://wd.gzmigu.cn

Py:   class Admin(User): pass
来源：http://dx.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://qx.shxzskj.cn

JS:   class Admin extends User {}
来源：http://gm.9csxet.cn

TS:   class Admin extends User {}
来源：http://tq.newstarts.cn

Java: class Admin extends User {}
来源：http://iz.lnxyls.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wo.asd995.cn

Ruby: class Admin < User; end
来源：http://ss.9csxet.cn

C#:   class Admin : User {}
来源：http://su.shtwfgs.cn

[G06] 重写方法
来源：http://oj.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://gi.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dq.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://hw.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://dj.shxzukj.cn

Java: @Override String greet() { return "admin"; }
来源：http://ms.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vy.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://ef.chemitech.net.cn


<!-- 参考信息 -->