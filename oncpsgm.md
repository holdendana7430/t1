代发 wailian999

Go:   strings.Join(items, ",")
来源：http://rf.hahajie.cn

Ruby: items.join(",")
来源：http://dc.hnjuh.cn

C#:   string.Join(",", items)
来源：http://aq.shxzukj.cn

[E09] 去除所有空白字符
来源：http://yi.shxzukj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://de.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://od.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://og.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://se.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://im.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mz.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ya.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wy.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://bl.yuexingan06.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://iv.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hw.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://ek.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://sa.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://fn.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nm.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rk.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bx.newstarts.cn

[E11] 反转字符串
来源：http://kf.bjjhwx.cn

Py:   s[::-1]
来源：http://xp.gzmigu.cn

PHP:  strrev($s);
来源：http://vr.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://ay.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://lc.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ah.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lb.panjiajie.cn

Ruby: s.reverse
来源：http://sy.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mn.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://om.wgjwhj.cn

Py:   s.count("a")
来源：http://iv.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://jk.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://tj.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://ab.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ph.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://tu.huixiangedu.cn

Ruby: s.count("a")
来源：http://vp.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://qa.lnxyls.cn

[E13] 逐字符遍历
来源：http://pk.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://lg.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://df.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ir.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jf.9csxet.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cj.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tj.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gg.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wh.muxihuayi.cn

[E14] URL 编码与 Base64
来源：http://mq.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pb.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ul.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dm.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wc.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ie.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zs.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yu.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rm.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://cr.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kw.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zh.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lh.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cg.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rd.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ov.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qt.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xm.nicolike.cn

[E16] 数字千分位
来源：http://qd.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://cn.hahajie.cn

PHP:  number_format(1234567);
来源：http://rw.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ye.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wl.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jp.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://om.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mh.asd995.cn

C#:   1234567.ToString("N0")
来源：http://zp.asd995.cn

[E17] 首字母大写
来源：http://og.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dp.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ne.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qw.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ev.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ej.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yi.bjjhwx.cn

Ruby: s.capitalize
来源：http://pq.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bu.bjjhwx.cn

[E18] 模板占位符替换
来源：http://ie.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://df.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nl.shxzskj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vf.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rr.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kg.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pj.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iq.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vy.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://si.521024.cn

Py:   s.splitlines()
来源：http://yl.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ph.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://pf.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://jh.chemitech.net.cn

Java: s.lines().toList()
来源：http://wu.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://ti.gzmigu.cn

Ruby: s.lines
来源：http://tr.521024.cn

C#:   s.Split('\n')
来源：http://cd.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://cu.muxihuayi.cn

Py:   if not s:
来源：http://fh.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://um.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sw.muxihuayi.cn

TS:   if (s === "") {}
来源：http://xo.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://zm.shxzskj.cn

Go:   if s == "" {}
来源：http://qn.bjjhwx.cn

Ruby: if s.empty?
来源：http://qo.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sh.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://hg.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zi.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ls.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ny.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ku.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fs.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://vq.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sh.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dj.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://mm.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rs.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ti.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mf.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iw.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ld.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qu.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://up.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kc.huanxung.cn

================================================================================
来源：http://us.yuntaijiaju.cn

F. 文件与目录
来源：http://tq.521024.cn

================================================================================
来源：http://to.jctech888.com.cn

[F01] 读取整个文件
来源：http://bs.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dr.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://ec.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zs.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fx.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://og.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rd.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://kp.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://aa.wgjwhj.cn

[F02] 逐行读取文件
来源：http://ph.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lm.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pq.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gu.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jq.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xk.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mn.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nx.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://he.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://ya.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rk.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yo.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xl.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mf.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ja.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cl.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://zx.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hf.nicolike.cn

[F04] 追加写入文件
来源：http://ne.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gy.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zx.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ps.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yq.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ja.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nh.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ez.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zy.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://dq.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ji.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://lv.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://ix.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://bx.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ic.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lj.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://nd.asd995.cn

C#:   File.Exists("a.txt")
来源：http://zb.wgjwhj.cn

[F06] 删除文件
来源：http://gb.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://ml.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://jz.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ah.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://md.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pu.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://ch.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://bp.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://rm.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://xm.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qi.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cv.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fn.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gw.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://um.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ty.hnjuh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hl.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://op.panjiajie.cn

[F08] 遍历目录
来源：http://gf.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sl.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://os.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://ls.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://kb.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://to.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fm.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://yq.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://su.hnjuh.cn

[F09] 获取文件大小
来源：http://hk.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://ds.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://fu.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://av.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://ax.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pk.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ub.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://fd.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://pj.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://ki.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wg.jctech888.com.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wt.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ir.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://gf.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ap.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bv.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qi.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iv.shxzukj.cn

[F11] 复制与移动文件
来源：http://oq.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://la.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jn.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rm.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pc.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tz.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gi.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vo.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sq.jctech888.com.cn

[F12] CSV 读写
来源：http://mt.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://no.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vi.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bi.jianghongdianzi.cn

TS:   // 同上
来源：http://pr.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ch.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nf.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jp.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cv.chemitech.net.cn

================================================================================
来源：http://zb.panjiajie.cn

G. 面向对象
来源：http://pu.shxzukj.cn

================================================================================
来源：http://hc.haigaiapp.cn

[G01] 定义类
来源：http://eb.asd995.cn

Py:   class User: pass
来源：http://sy.yuexingan06.cn

PHP:  class User {}
来源：http://kw.521024.cn

JS:   class User {}
来源：http://dx.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://xk.nicolike.cn

Java: class User {}
来源：http://hz.panjiajie.cn

Go:   type User struct { Name string }
来源：http://kw.huixiangedu.cn

Ruby: class User; end
来源：http://ii.panjiajie.cn

C#:   class User {}
来源：http://hn.bjjhwx.cn

[G02] 构造函数
来源：http://yo.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://au.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://sw.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://bb.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://wr.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://xv.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ie.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://tx.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://po.nszjky.cn

[G03] 实例属性
来源：http://kt.jctech888.com.cn

Py:   self.name = "x"
来源：http://tf.nicolike.cn

PHP:  public string $name = "x";
来源：http://og.shtwfgs.cn

JS:   this.name = "x";
来源：http://ec.521024.cn

TS:   name: string = "x";
来源：http://pa.nicolike.cn

Java: private String name;
来源：http://sv.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://se.szsharing.cn

Ruby: @name = "x"
来源：http://xi.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://ok.nszjky.cn

[G04] 定义方法
来源：http://jm.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://qn.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tl.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://mz.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://hl.panjiajie.cn

Java: String greet() { return name; }
来源：http://al.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://us.szsharing.cn

Ruby: def greet; @name; end
来源：http://ve.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://ar.shtwfgs.cn

[G05] 继承
来源：http://oh.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://yu.szsharing.cn

PHP:  class Admin extends User {}
来源：http://vb.hnjuh.cn

JS:   class Admin extends User {}
来源：http://ba.szsharing.cn

TS:   class Admin extends User {}
来源：http://ri.nszjky.cn

Java: class Admin extends User {}
来源：http://tv.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lq.newstarts.cn

Ruby: class Admin < User; end
来源：http://yc.jctech888.com.cn

C#:   class Admin : User {}
来源：http://sw.chemitech.net.cn

[G06] 重写方法
来源：http://mu.haigaiapp.cn

Py:   def greet(self): return "admin"
来源：http://tl.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sm.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://nn.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://oh.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://cf.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zm.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://ox.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://pb.szxytkj.cn

[G07] 调用父类方法
来源：http://ze.bjjhwx.cn

Py:   super().greet()
来源：http://hl.chemitech.net.cn

PHP:  parent::greet();
来源：http://go.9csxet.cn


<!-- 参考信息 -->