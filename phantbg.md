代发 wailian999

Go:   strings.Join(items, ",")
来源：http://wx.521024.cn

Ruby: items.join(",")
来源：http://dv.huanxung.cn

C#:   string.Join(",", items)
来源：http://ba.9csxet.cn

[E09] 去除所有空白字符
来源：http://dk.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ob.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bd.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://di.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://fi.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://qg.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://br.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://iy.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zb.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://xs.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gq.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mh.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://ve.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://fn.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://fg.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tm.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ty.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qb.huanxung.cn

[E11] 反转字符串
来源：http://st.yuexingan06.cn

Py:   s[::-1]
来源：http://xc.nicolike.cn

PHP:  strrev($s);
来源：http://cr.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://bs.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://wv.colortex.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dl.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pl.hnjuh.cn

Ruby: s.reverse
来源：http://qt.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dk.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://zl.521024.cn

Py:   s.count("a")
来源：http://nm.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://du.huanxung.cn

JS:   s.split("a").length - 1
来源：http://eb.asd995.cn

TS:   s.split("a").length - 1
来源：http://jd.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zj.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://sy.chemitech.net.cn

Ruby: s.count("a")
来源：http://an.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://un.huanxung.cn

[E13] 逐字符遍历
来源：http://wy.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://xg.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ef.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xe.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ei.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ey.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nk.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://az.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wz.shxzskj.cn

[E14] URL 编码与 Base64
来源：http://hr.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cs.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gy.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bo.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://in.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jb.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ae.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nx.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pm.colortex.cn

[E15] HTML 转义 / 反转义
来源：http://jr.bjjhwx.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ah.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gx.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jk.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dy.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yg.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rg.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nx.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fr.jianghongdianzi.cn

[E16] 数字千分位
来源：http://io.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://xg.shxzukj.cn

PHP:  number_format(1234567);
来源：http://bo.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cf.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xu.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nn.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nh.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fq.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://uj.yuntaijiaju.cn

[E17] 首字母大写
来源：http://fx.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cj.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ra.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ws.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hg.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ut.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ql.521024.cn

Ruby: s.capitalize
来源：http://pz.huixinmuqiang.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lo.521024.cn

[E18] 模板占位符替换
来源：http://vo.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xl.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ih.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ml.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xt.gzmigu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eh.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tg.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kh.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nc.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://id.521024.cn

Py:   s.splitlines()
来源：http://rf.nicolike.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pf.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://uy.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://fx.nicolike.cn

Java: s.lines().toList()
来源：http://sn.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://ue.yuexingan06.cn

Ruby: s.lines
来源：http://vi.huanxung.cn

C#:   s.Split('\n')
来源：http://si.shxzskj.cn

[E20] 判断字符串是否为空
来源：http://ii.szxytkj.cn

Py:   if not s:
来源：http://ry.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://df.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hg.newstarts.cn

TS:   if (s === "") {}
来源：http://bj.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://al.521024.cn

Go:   if s == "" {}
来源：http://rt.asd995.cn

Ruby: if s.empty?
来源：http://wp.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qw.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://ui.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oc.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zi.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ex.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pt.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yw.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://tz.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oa.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jq.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://rs.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zz.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ht.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ss.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ay.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nz.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bh.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://as.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wt.huanxung.cn

================================================================================
来源：http://wa.hahajie.cn

F. 文件与目录
来源：http://iw.asd995.cn

================================================================================
来源：http://pk.asd995.cn

[F01] 读取整个文件
来源：http://kn.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tt.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://fq.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kj.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ux.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://au.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yt.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://uk.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://ap.newstarts.cn

[F02] 逐行读取文件
来源：http://jw.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tb.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xh.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dx.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fd.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ui.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ce.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ib.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vf.bookmarksfly.cn

[F03] 写入文件（覆盖）
来源：http://zb.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gn.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://es.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://if.newstarts.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xy.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gw.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ja.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://py.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cg.nicolike.cn

[F04] 追加写入文件
来源：http://sz.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vh.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tp.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kg.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vv.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bj.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hu.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wa.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://au.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://cr.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hb.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://ev.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://ch.jianghongdianzi.cn

TS:   fs.existsSync("a.txt")
来源：http://cq.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ex.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fm.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://zp.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://ak.jianghongdianzi.cn

[F06] 删除文件
来源：http://ri.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://si.521024.cn

PHP:  unlink("a.txt");
来源：http://kh.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ep.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tz.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aw.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://et.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://hj.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://nu.nszjky.cn

[F07] 创建目录（含多级）
来源：http://fp.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dh.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qp.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vn.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mh.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qj.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://st.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yr.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sf.huanxung.cn

[F08] 遍历目录
来源：http://of.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hm.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mp.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://st.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://au.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nq.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zr.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://ps.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://nc.hahajie.cn

[F09] 获取文件大小
来源：http://tx.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://dc.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://xt.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://zr.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://vn.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://js.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sm.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://zq.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://je.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://wi.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sa.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://df.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ax.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://ck.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ku.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mx.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vs.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ud.huixiangedu.cn

[F11] 复制与移动文件
来源：http://hq.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mo.shxzukj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kz.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jv.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gy.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hx.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kw.shtwfgs.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://va.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dz.huanxung.cn

[F12] CSV 读写
来源：http://gc.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vt.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pg.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xn.panjiajie.cn

TS:   // 同上
来源：http://cn.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oz.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hm.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fe.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://on.nicolike.cn

================================================================================
来源：http://de.bookmarksfly.cn

G. 面向对象
来源：http://xc.jianghongdianzi.cn

================================================================================
来源：http://so.bjjhwx.cn

[G01] 定义类
来源：http://bw.yuexingan06.cn

Py:   class User: pass
来源：http://ks.bookmarksfly.cn

PHP:  class User {}
来源：http://ji.jianghongdianzi.cn

JS:   class User {}
来源：http://rq.asd995.cn

TS:   class User { name: string = ""; }
来源：http://iz.asd995.cn

Java: class User {}
来源：http://ml.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://gf.gzmigu.cn

Ruby: class User; end
来源：http://vj.szxytkj.cn

C#:   class User {}
来源：http://am.yuntaijiaju.cn

[G02] 构造函数
来源：http://fq.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://gm.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://xq.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://ij.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://zp.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://mb.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cg.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://gh.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://dj.bookmarksfly.cn

[G03] 实例属性
来源：http://zf.shtwfgs.cn

Py:   self.name = "x"
来源：http://hw.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://ox.szxytkj.cn

JS:   this.name = "x";
来源：http://ak.shxzskj.cn

TS:   name: string = "x";
来源：http://mb.gzmigu.cn

Java: private String name;
来源：http://un.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://io.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://gc.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://io.shtwfgs.cn

[G04] 定义方法
来源：http://db.newstarts.cn

Py:   def greet(self): return self.name
来源：http://gq.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pk.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://tt.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://zi.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://ew.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gl.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://dx.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://tn.newstarts.cn

[G05] 继承
来源：http://hk.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://ji.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://wz.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://lf.hahajie.cn

TS:   class Admin extends User {}
来源：http://lm.hahajie.cn

Java: class Admin extends User {}
来源：http://ac.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bm.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://eh.yuexingan06.cn

C#:   class Admin : User {}
来源：http://am.yuntaijiaju.cn

[G06] 重写方法
来源：http://sm.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://ih.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fi.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://gk.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://um.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://iy.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bn.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://bs.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://yk.jctech888.com.cn

[G07] 调用父类方法
来源：http://xp.9csxet.cn

Py:   super().greet()
来源：http://tu.gzmigu.cn

PHP:  parent::greet();
来源：http://iy.shtwfgs.cn


<!-- 参考信息 -->