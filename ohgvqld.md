代发 wailian999

Go:   strings.Join(items, ",")
来源：http://mb.jctech888.com.cn

Ruby: items.join(",")
来源：http://zt.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://zl.nicolike.cn

[E09] 去除所有空白字符
来源：http://on.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://au.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ff.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://mb.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://uc.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://ab.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gj.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lc.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cm.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://od.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ij.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tn.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://ma.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://ro.colortex.cn

Java: String.format("%03d", 7)
来源：http://kf.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sx.shxzskj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xj.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dj.bookmarksfly.cn

[E11] 反转字符串
来源：http://or.yuexingan06.cn

Py:   s[::-1]
来源：http://hq.newstarts.cn

PHP:  strrev($s);
来源：http://qj.521024.cn

JS:   [...s].reverse().join("")
来源：http://ib.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://zw.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gk.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bf.chemitech.net.cn

Ruby: s.reverse
来源：http://af.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://et.newstarts.cn

[E12] 统计某字符出现次数
来源：http://qm.gzmigu.cn

Py:   s.count("a")
来源：http://gh.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://gn.yuexingan06.cn

JS:   s.split("a").length - 1
来源：http://tr.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://ib.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tu.asd995.cn

Go:   strings.Count(s, "a")
来源：http://zj.colortex.cn

Ruby: s.count("a")
来源：http://jn.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://mo.bjjhwx.cn

[E13] 逐字符遍历
来源：http://yr.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://cl.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://an.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bh.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jg.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lh.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qm.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xv.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://om.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://jj.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pm.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bh.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ra.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nv.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hg.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xk.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yg.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ip.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://wf.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jj.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ki.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ol.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qk.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ju.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://za.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gq.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dz.huixiangedu.cn

[E16] 数字千分位
来源：http://rn.newstarts.cn

Py:   f"{1234567:,}"
来源：http://cu.huanxung.cn

PHP:  number_format(1234567);
来源：http://em.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lm.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pa.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lh.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://re.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ny.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://th.hnjuh.cn

[E17] 首字母大写
来源：http://bu.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fx.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jn.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aq.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://no.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dx.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gl.huixiangedu.cn

Ruby: s.capitalize
来源：http://ls.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ui.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://ap.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fl.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://po.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fm.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pm.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fz.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wy.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xk.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rw.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://tl.hnjuh.cn

Py:   s.splitlines()
来源：http://xi.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://co.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://jq.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://qc.shxzukj.cn

Java: s.lines().toList()
来源：http://mr.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://ml.chemitech.net.cn

Ruby: s.lines
来源：http://kw.chemitech.net.cn

C#:   s.Split('\n')
来源：http://pw.newstarts.cn

[E20] 判断字符串是否为空
来源：http://ev.panjiajie.cn

Py:   if not s:
来源：http://ot.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pa.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zy.gzmigu.cn

TS:   if (s === "") {}
来源：http://ma.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://cm.nicolike.cn

Go:   if s == "" {}
来源：http://pf.bjjhwx.cn

Ruby: if s.empty?
来源：http://af.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ta.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://xb.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ti.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ls.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yx.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wn.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ny.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://vr.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yv.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rc.nicolike.cn

[E22] 字节长度与字符长度
来源：http://qs.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://up.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://on.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://im.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ew.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://df.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://un.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://ay.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dv.huixiangedu.cn

================================================================================
来源：http://gp.muxihuayi.cn

F. 文件与目录
来源：http://jh.yuntaijiaju.cn

================================================================================
来源：http://gd.newstarts.cn

[F01] 读取整个文件
来源：http://tp.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iz.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://zw.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ie.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ng.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://br.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lw.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://dw.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://pp.szxytkj.cn

[F02] 逐行读取文件
来源：http://us.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jk.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://of.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tn.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oa.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jk.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vr.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hi.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ur.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://da.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nc.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fg.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bn.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vb.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ik.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ch.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://vp.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vp.szxytkj.cn

[F04] 追加写入文件
来源：http://hd.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ef.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qs.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ua.wgjwhj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xk.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xy.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ie.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dw.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mb.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://kr.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cd.colortex.cn

PHP:  file_exists("a.txt");
来源：http://fe.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://yu.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://nb.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ln.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ag.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://wj.nicolike.cn

C#:   File.Exists("a.txt")
来源：http://pw.hnjuh.cn

[F06] 删除文件
来源：http://yl.huanxung.cn

Py:   os.remove("a.txt")
来源：http://or.huixinmuqiang.cn

PHP:  unlink("a.txt");
来源：http://jz.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ox.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://or.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jo.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://jy.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://df.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://vw.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://dm.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hm.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ap.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mn.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kq.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rv.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ef.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qa.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uv.9csxet.cn

[F08] 遍历目录
来源：http://qe.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lq.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ar.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://he.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://cu.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jk.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qm.newstarts.cn

Ruby: Dir.children("dir")
来源：http://aq.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://dx.szxytkj.cn

[F09] 获取文件大小
来源：http://oh.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://ye.asd995.cn

PHP:  filesize("a.txt");
来源：http://oa.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://kb.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://ds.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ja.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pf.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://cw.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://yj.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://zf.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zg.jctech888.com.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://de.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lx.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://xu.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dd.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jq.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pj.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qi.hnjuh.cn

[F11] 复制与移动文件
来源：http://jy.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rd.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ei.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ed.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iz.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dz.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xc.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dt.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://al.bjjhwx.cn

[F12] CSV 读写
来源：http://gg.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://to.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nk.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uv.panjiajie.cn

TS:   // 同上
来源：http://sx.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wp.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nt.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ew.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nm.szsharing.cn

================================================================================
来源：http://ho.shxzukj.cn

G. 面向对象
来源：http://br.bookmarksfly.cn

================================================================================
来源：http://nr.colortex.cn

[G01] 定义类
来源：http://eh.muxihuayi.cn

Py:   class User: pass
来源：http://tr.521024.cn

PHP:  class User {}
来源：http://xw.nszjky.cn

JS:   class User {}
来源：http://xe.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://ta.asd995.cn

Java: class User {}
来源：http://gk.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://fm.huixinmuqiang.cn

Ruby: class User; end
来源：http://yo.bookmarksfly.cn

C#:   class User {}
来源：http://jg.szsharing.cn

[G02] 构造函数
来源：http://it.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://ne.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://qa.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://bv.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://gm.shtwfgs.cn

Java: User(String name) { this.name = name; }
来源：http://pq.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ct.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://rr.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://jq.shtwfgs.cn

[G03] 实例属性
来源：http://vz.asd995.cn

Py:   self.name = "x"
来源：http://pb.9csxet.cn

PHP:  public string $name = "x";
来源：http://tp.chemitech.net.cn

JS:   this.name = "x";
来源：http://ko.chemitech.net.cn

TS:   name: string = "x";
来源：http://hw.asd995.cn

Java: private String name;
来源：http://ai.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eo.newstarts.cn

Ruby: @name = "x"
来源：http://at.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://ou.haigaiapp.cn

[G04] 定义方法
来源：http://pc.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://gc.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mw.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://sp.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://lq.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://ky.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kb.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://qn.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://zy.chemitech.net.cn

[G05] 继承
来源：http://dl.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://vb.szsharing.cn

PHP:  class Admin extends User {}
来源：http://uu.shxzskj.cn

JS:   class Admin extends User {}
来源：http://cg.hahajie.cn

TS:   class Admin extends User {}
来源：http://uh.newstarts.cn

Java: class Admin extends User {}
来源：http://sa.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ma.asd995.cn

Ruby: class Admin < User; end
来源：http://fp.bjjhwx.cn

C#:   class Admin : User {}
来源：http://ys.hnjuh.cn

[G06] 重写方法
来源：http://yr.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://ld.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ui.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://gt.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://pg.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://wb.asd995.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gt.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://jk.9csxet.cn

C#:   public override string Greet() => "admin";
来源：http://zd.huixiangedu.cn

[G07] 调用父类方法
来源：http://cg.newstarts.cn

Py:   super().greet()
来源：http://cm.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://ao.yuexingan06.cn


<!-- 参考信息 -->