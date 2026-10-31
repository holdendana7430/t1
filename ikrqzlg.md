代发 wailian999

PHP:  implode(",", $items);
来源：http://en.hahajie.cn

JS:   items.join(",")
来源：http://yg.nszjky.cn

TS:   items.join(",")
来源：http://xw.jctech888.com.cn

Java: String.join(",", items)
来源：http://or.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://vs.nszjky.cn

Ruby: items.join(",")
来源：http://gf.colortex.cn

C#:   string.Join(",", items)
来源：http://qn.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://uk.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zc.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ul.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://hh.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://ym.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://ze.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://te.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://az.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fz.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://zu.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://io.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yb.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://nw.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://gh.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://gn.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wg.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vj.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hk.jctech888.com.cn

[E11] 反转字符串
来源：http://pg.hnjuh.cn

Py:   s[::-1]
来源：http://ec.wgjwhj.cn

PHP:  strrev($s);
来源：http://ba.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://nm.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://qj.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qi.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hb.yuexingan06.cn

Ruby: s.reverse
来源：http://gf.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tp.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://mc.huanxung.cn

Py:   s.count("a")
来源：http://iu.colortex.cn

PHP:  substr_count($s, "a");
来源：http://iy.szsharing.cn

JS:   s.split("a").length - 1
来源：http://mb.nicolike.cn

TS:   s.split("a").length - 1
来源：http://iq.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xh.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://ak.hahajie.cn

Ruby: s.count("a")
来源：http://lo.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://rl.newstarts.cn

[E13] 逐字符遍历
来源：http://mz.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://bp.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ko.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nq.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kr.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ju.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kf.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pw.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rl.521024.cn

[E14] URL 编码与 Base64
来源：http://cn.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gy.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zu.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mk.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://id.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qg.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://an.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oi.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cm.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://ss.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ep.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hk.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bj.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gu.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ux.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gy.bookmarksfly.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tn.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ct.asd995.cn

[E16] 数字千分位
来源：http://wo.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://uz.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://fo.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ge.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://al.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cm.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xg.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sy.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://rj.hahajie.cn

[E17] 首字母大写
来源：http://md.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aj.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pr.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ce.9csxet.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cz.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ox.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ej.521024.cn

Ruby: s.capitalize
来源：http://ip.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pr.huixiangedu.cn

[E18] 模板占位符替换
来源：http://ks.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jp.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zz.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://om.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cs.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hg.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wn.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ww.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yz.asd995.cn

[E19] 多行文本按行拆分
来源：http://nd.panjiajie.cn

Py:   s.splitlines()
来源：http://uy.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vu.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://ip.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://dx.panjiajie.cn

Java: s.lines().toList()
来源：http://ih.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://lv.521024.cn

Ruby: s.lines
来源：http://ij.shtwfgs.cn

C#:   s.Split('\n')
来源：http://rf.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://fz.jctech888.com.cn

Py:   if not s:
来源：http://du.huixinmuqiang.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yt.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ce.hnjuh.cn

TS:   if (s === "") {}
来源：http://sc.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://eu.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://lx.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://tr.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vz.521024.cn

[E21] 超长截断加省略号
来源：http://ow.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hk.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://di.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rw.hnjuh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://by.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wg.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://gn.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vi.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cp.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://fd.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ve.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pw.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xx.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jz.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hs.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fg.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://oa.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wn.jianghongdianzi.cn

================================================================================
来源：http://hv.huanxung.cn

F. 文件与目录
来源：http://kn.nszjky.cn

================================================================================
来源：http://wx.hahajie.cn

[F01] 读取整个文件
来源：http://cm.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jl.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://oj.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ui.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gg.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vp.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pm.hahajie.cn

Ruby: File.read("a.txt")
来源：http://nk.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://zf.nszjky.cn

[F02] 逐行读取文件
来源：http://zz.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oo.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ad.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bn.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ca.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yg.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ab.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mr.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uj.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://dd.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kp.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://uc.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dz.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dj.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yo.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dy.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://bd.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dn.huanxung.cn

[F04] 追加写入文件
来源：http://pl.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qg.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://or.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hb.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jp.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sc.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oc.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://az.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fn.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://zd.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ee.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://qh.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://ih.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://mn.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tg.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ox.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://db.colortex.cn

C#:   File.Exists("a.txt")
来源：http://ql.wgjwhj.cn

[F06] 删除文件
来源：http://ma.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://dm.521024.cn

PHP:  unlink("a.txt");
来源：http://ye.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xu.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kl.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://th.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://aa.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://mk.asd995.cn

C#:   File.Delete("a.txt");
来源：http://nj.newstarts.cn

[F07] 创建目录（含多级）
来源：http://sd.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xw.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gr.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lc.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zh.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jz.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ju.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zt.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://be.haigaiapp.cn

[F08] 遍历目录
来源：http://ad.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rn.yuntaijiaju.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vl.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://lq.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://uf.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kb.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fa.huanxung.cn

Ruby: Dir.children("dir")
来源：http://ao.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://ut.huixiangedu.cn

[F09] 获取文件大小
来源：http://cw.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://wb.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://rz.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://la.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://cz.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pk.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bp.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://hm.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://ew.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://dc.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yv.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cs.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qq.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://ty.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sb.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ks.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ah.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zl.huixiangedu.cn

[F11] 复制与移动文件
来源：http://ug.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cp.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vd.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uu.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gy.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://so.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ku.shtwfgs.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gv.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mm.huixiangedu.cn

[F12] CSV 读写
来源：http://fs.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fo.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ci.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cg.bjjhwx.cn

TS:   // 同上
来源：http://qa.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yb.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lf.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gx.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cw.huixiangedu.cn

================================================================================
来源：http://df.shxzukj.cn

G. 面向对象
来源：http://be.yuexingan06.cn

================================================================================
来源：http://lz.szxytkj.cn

[G01] 定义类
来源：http://it.panjiajie.cn

Py:   class User: pass
来源：http://sn.9csxet.cn

PHP:  class User {}
来源：http://ws.colortex.cn

JS:   class User {}
来源：http://hc.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://lh.gzmigu.cn

Java: class User {}
来源：http://bq.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://uc.nszjky.cn

Ruby: class User; end
来源：http://zv.szsharing.cn

C#:   class User {}
来源：http://tm.yuntaijiaju.cn

[G02] 构造函数
来源：http://qv.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://er.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://hh.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://nd.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://sk.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://bb.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ey.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://xt.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://vx.shtwfgs.cn

[G03] 实例属性
来源：http://qy.yuexingan06.cn

Py:   self.name = "x"
来源：http://zv.szxytkj.cn

PHP:  public string $name = "x";
来源：http://ow.huixiangedu.cn

JS:   this.name = "x";
来源：http://xm.hahajie.cn

TS:   name: string = "x";
来源：http://cr.yuexingan06.cn

Java: private String name;
来源：http://us.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mk.9csxet.cn

Ruby: @name = "x"
来源：http://uk.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://ka.521024.cn

[G04] 定义方法
来源：http://bm.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://yz.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://je.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://si.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://jz.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://ji.shxzskj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sk.hnjuh.cn

Ruby: def greet; @name; end
来源：http://we.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://tf.bjjhwx.cn

[G05] 继承
来源：http://tj.lnxyls.cn

Py:   class Admin(User): pass
来源：http://vm.9csxet.cn

PHP:  class Admin extends User {}
来源：http://mo.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://vv.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://va.jctech888.com.cn

Java: class Admin extends User {}
来源：http://no.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bi.huanxung.cn

Ruby: class Admin < User; end
来源：http://ms.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://mk.nicolike.cn

[G06] 重写方法
来源：http://pd.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://nb.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://js.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://yr.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://jl.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://nb.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oe.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://gq.hnjuh.cn


<!-- 参考信息 -->