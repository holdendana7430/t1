代发 wailian999

Go:   strings.Join(items, ",")
来源：http://fh.yuexingan06.cn

Ruby: items.join(",")
来源：http://ow.521024.cn

C#:   string.Join(",", items)
来源：http://og.shxzukj.cn

[E09] 去除所有空白字符
来源：http://ti.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mx.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://et.bookmarksfly.cn

JS:   s.replace(/\s+/g, "")
来源：http://fk.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://vr.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://gp.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mb.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tp.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://me.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://lp.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wc.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ee.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://ly.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://ju.9csxet.cn

Java: String.format("%03d", 7)
来源：http://nd.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fk.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://is.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qi.huixinmuqiang.cn

[E11] 反转字符串
来源：http://vs.newstarts.cn

Py:   s[::-1]
来源：http://qi.newstarts.cn

PHP:  strrev($s);
来源：http://pp.colortex.cn

JS:   [...s].reverse().join("")
来源：http://ta.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://ws.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ad.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mr.shxzukj.cn

Ruby: s.reverse
来源：http://zh.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vg.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://tn.szsharing.cn

Py:   s.count("a")
来源：http://li.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://rt.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://sb.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://ff.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rc.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://pm.shxzukj.cn

Ruby: s.count("a")
来源：http://qr.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://ad.haigaiapp.cn

[E13] 逐字符遍历
来源：http://xf.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://oj.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rk.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qa.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wv.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qn.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://iz.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hn.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ys.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://hh.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cp.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qm.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cb.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ds.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rj.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iq.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dc.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://is.newstarts.cn

[E15] HTML 转义 / 反转义
来源：http://nv.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bw.haigaiapp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://aj.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wl.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ib.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ne.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dk.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://er.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lj.huixiangedu.cn

[E16] 数字千分位
来源：http://yz.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://kj.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://sy.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pz.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://la.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eo.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://df.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hn.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://hx.jianghongdianzi.cn

[E17] 首字母大写
来源：http://mv.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cd.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hw.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sc.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rc.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ep.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dq.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://fo.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tv.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://jx.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kr.shtwfgs.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nk.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ad.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pt.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pw.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gm.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wj.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zv.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://ce.hnjuh.cn

Py:   s.splitlines()
来源：http://ue.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hr.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://ai.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://wj.asd995.cn

Java: s.lines().toList()
来源：http://rv.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://gg.colortex.cn

Ruby: s.lines
来源：http://ak.shtwfgs.cn

C#:   s.Split('\n')
来源：http://nv.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://yh.521024.cn

Py:   if not s:
来源：http://hf.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xl.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uc.panjiajie.cn

TS:   if (s === "") {}
来源：http://py.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://ex.shxzukj.cn

Go:   if s == "" {}
来源：http://ya.colortex.cn

Ruby: if s.empty?
来源：http://ua.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kq.gzmigu.cn

[E21] 超长截断加省略号
来源：http://ur.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qx.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xu.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rv.haigaiapp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ks.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nk.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://bx.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bn.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fb.nszjky.cn

[E22] 字节长度与字符长度
来源：http://yf.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://km.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ch.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ze.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://di.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tu.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://ql.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cg.muxihuayi.cn

================================================================================
来源：http://uv.nszjky.cn

F. 文件与目录
来源：http://pe.bookmarksfly.cn

================================================================================
来源：http://wh.shtwfgs.cn

[F01] 读取整个文件
来源：http://zp.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mu.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://js.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vu.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zt.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hc.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jj.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://md.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://sg.haigaiapp.cn

[F02] 逐行读取文件
来源：http://rt.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lk.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wb.bjjhwx.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uq.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oy.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://no.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wy.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://he.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://du.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://ev.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ru.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gn.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sa.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ab.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yh.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kx.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://yo.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lw.huanxung.cn

[F04] 追加写入文件
来源：http://xn.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jw.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zk.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pk.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xk.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vo.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nw.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ls.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ik.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://vr.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yr.szxytkj.cn

PHP:  file_exists("a.txt");
来源：http://gl.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://wd.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://mt.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jq.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mr.shtwfgs.cn

Ruby: File.exist?("a.txt")
来源：http://bx.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://nx.szsharing.cn

[F06] 删除文件
来源：http://br.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://no.colortex.cn

PHP:  unlink("a.txt");
来源：http://ir.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vx.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fw.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gg.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://lw.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://ds.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://be.szsharing.cn

[F07] 创建目录（含多级）
来源：http://sm.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gu.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tj.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bf.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://by.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hm.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ie.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wd.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zs.panjiajie.cn

[F08] 遍历目录
来源：http://ha.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://so.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bq.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://ix.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://xq.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dy.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ff.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://yo.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://xv.shtwfgs.cn

[F09] 获取文件大小
来源：http://om.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://cl.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://wr.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://st.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://wz.bookmarksfly.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vn.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://of.newstarts.cn

Ruby: File.size("a.txt")
来源：http://wk.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://ac.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://hb.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oc.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lm.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hn.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://wv.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cf.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fc.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://on.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ky.shxzskj.cn

[F11] 复制与移动文件
来源：http://sc.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ra.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gy.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://np.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nb.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pk.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ng.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bf.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ps.szsharing.cn

[F12] CSV 读写
来源：http://ml.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://el.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ly.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bk.yuexingan06.cn

TS:   // 同上
来源：http://bx.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tk.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pc.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tu.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mv.huanxung.cn

================================================================================
来源：http://mo.panjiajie.cn

G. 面向对象
来源：http://zc.haigaiapp.cn

================================================================================
来源：http://za.521024.cn

[G01] 定义类
来源：http://vb.9csxet.cn

Py:   class User: pass
来源：http://fu.huixiangedu.cn

PHP:  class User {}
来源：http://qv.jianghongdianzi.cn

JS:   class User {}
来源：http://pj.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://mr.yuexingan06.cn

Java: class User {}
来源：http://wp.nicolike.cn

Go:   type User struct { Name string }
来源：http://vh.hnjuh.cn

Ruby: class User; end
来源：http://ml.colortex.cn

C#:   class User {}
来源：http://ik.shtwfgs.cn

[G02] 构造函数
来源：http://jf.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://et.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://be.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://fe.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://pd.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://qy.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jg.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://yz.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://wl.jctech888.com.cn

[G03] 实例属性
来源：http://ci.shxzukj.cn

Py:   self.name = "x"
来源：http://wv.gzmigu.cn

PHP:  public string $name = "x";
来源：http://aq.hahajie.cn

JS:   this.name = "x";
来源：http://ec.szxytkj.cn

TS:   name: string = "x";
来源：http://kk.bjjhwx.cn

Java: private String name;
来源：http://hm.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ju.jctech888.com.cn

Ruby: @name = "x"
来源：http://pw.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://af.hahajie.cn

[G04] 定义方法
来源：http://bz.521024.cn

Py:   def greet(self): return self.name
来源：http://ty.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ol.asd995.cn

JS:   greet() { return this.name; }
来源：http://om.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://oy.wgjwhj.cn

Java: String greet() { return name; }
来源：http://pn.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ix.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://rf.huanxung.cn

C#:   public string Greet() => Name;
来源：http://vo.shxzskj.cn

[G05] 继承
来源：http://vv.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://sc.szsharing.cn

PHP:  class Admin extends User {}
来源：http://pv.bjjhwx.cn

JS:   class Admin extends User {}
来源：http://mi.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://nn.yuexingan06.cn

Java: class Admin extends User {}
来源：http://fq.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gl.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://uu.newstarts.cn

C#:   class Admin : User {}
来源：http://eg.colortex.cn

[G06] 重写方法
来源：http://tz.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://dn.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vb.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://qu.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://ry.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://sw.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ge.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://sh.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://ay.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://ga.lnxyls.cn

Py:   super().greet()
来源：http://wm.jctech888.com.cn

PHP:  parent::greet();
来源：http://ji.gzmigu.cn


<!-- 参考信息 -->